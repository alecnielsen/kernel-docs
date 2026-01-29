# Common Operations

Code examples for frequent API operations.

## Setup

### Python SDK Setup

```python
from kernel import KernelClient
import os

# Initialize client with token
client = KernelClient(token=os.environ["KERNEL_TOKEN"])

# Or with explicit base URL
client = KernelClient(
    token=os.environ["KERNEL_TOKEN"],
    base_url="https://kernel.asimov.com"
)
```

## Constructs

### List Constructs

```python
# List all constructs in a repository
constructs = client.list_constructs(
    repository_id="repo-uuid",
    limit=100
)

for construct in constructs:
    print(f"{construct.name}: {len(construct.sequence)} bp")
```

### Get Construct Details

```python
# Get a specific construct
construct = client.get_construct(construct_id="construct-uuid")

print(f"Name: {construct.name}")
print(f"Length: {len(construct.sequence)} bp")
print(f"Annotations: {len(construct.annotations)}")
```

### Create Construct

```python
# Create a new construct
construct = client.create_construct(
    name="My New Construct",
    sequence="ATGCATGCATGC...",
    repository_id="repo-uuid",
    topology="circular",
    description="Expression vector for GFP"
)

print(f"Created: {construct.id}")
```

### Update Construct

```python
# Update construct properties
client.update_construct(
    construct_id="construct-uuid",
    name="Updated Name",
    description="New description"
)
```

### Export Construct

```python
# Export as GenBank
genbank_content = client.export_construct(
    construct_id="construct-uuid",
    format="genbank"
)

# Save to file
with open("construct.gb", "w") as f:
    f.write(genbank_content)
```

## Parts

### List Parts

```python
# List parts in a repository
parts = client.list_parts(
    repository_id="repo-uuid",
    part_type="promoter"  # Optional filter
)

for part in parts:
    print(f"{part.name} ({part.type})")
```

### Create Part

```python
# Create a new part
part = client.create_part(
    name="T7 Promoter",
    sequence="TAATACGACTCACTATAGGG",
    part_type="promoter",
    repository_id="repo-uuid"
)
```

### Search Parts

```python
# Search for parts
results = client.search_parts(
    query="CMV promoter",
    workspace_id="workspace-uuid"
)

for part in results:
    print(f"{part.name} in {part.repository.name}")
```

## Repositories

### List Repositories

```python
# Get all repositories
repos = client.list_repositories(workspace_id="workspace-uuid")

for repo in repos:
    print(f"{repo.name}: {repo.description}")
```

### Create Repository

```python
# Create a new repository
repo = client.create_repository(
    name="My Project",
    description="Antibody expression constructs",
    workspace_id="workspace-uuid"
)
```

## Search

### Global Search

```python
# Search across workspace
results = client.search(
    query="GFP expression",
    workspace_id="workspace-uuid",
    types=["construct", "part"]
)

for item in results:
    print(f"{item.type}: {item.name}")
```

### BLAST Search

```python
# BLAST a sequence
blast_results = client.blast(
    sequence="ATGGTGAGCAAGGGC...",
    database="workspace",  # or "public"
    workspace_id="workspace-uuid"
)

for hit in blast_results:
    print(f"{hit.name}: {hit.identity}% identity")
```

## Simulations

### Run Simulation

```python
# Start a simulation
run = client.run_simulation(
    construct_id="construct-uuid",
    parameters={
        "expression_system": "mammalian",
        "copy_number": 10
    }
)

print(f"Run ID: {run.id}")
print(f"Status: {run.status}")
```

### Check Run Status

```python
# Poll for completion
import time

while True:
    run = client.get_run(run_id=run.id)
    if run.status == "completed":
        break
    if run.status == "failed":
        raise Exception(f"Run failed: {run.error}")
    time.sleep(5)

# Get results
print(f"Results: {run.results}")
```

## Codon Optimization

### Optimize Sequence

```python
# Run codon optimization
result = client.optimize_codons(
    sequence="ATGGTGAGCAAG...",
    target_organism="cho",
    construct_id="construct-uuid"  # Optional
)

print(f"Optimized: {result.optimized_sequence}")
print(f"CAI improvement: {result.cai_before} -> {result.cai_after}")
```

## Error Handling

### Basic Error Handling

```python
from kernel.exceptions import KernelAPIError, NotFoundError

try:
    construct = client.get_construct("invalid-id")
except NotFoundError:
    print("Construct not found")
except KernelAPIError as e:
    print(f"API error: {e.message}")
```

### Rate Limit Handling

```python
import time
from kernel.exceptions import RateLimitError

def get_with_retry(construct_id, max_retries=3):
    for attempt in range(max_retries):
        try:
            return client.get_construct(construct_id)
        except RateLimitError as e:
            if attempt < max_retries - 1:
                time.sleep(e.retry_after)
            else:
                raise
```

## Batch Operations

### Bulk Export

```python
# Export multiple constructs
construct_ids = ["id1", "id2", "id3"]

for cid in construct_ids:
    content = client.export_construct(cid, format="genbank")
    with open(f"{cid}.gb", "w") as f:
        f.write(content)
```

### Bulk Create

```python
# Create multiple parts
parts_data = [
    {"name": "Promoter A", "sequence": "...", "type": "promoter"},
    {"name": "Promoter B", "sequence": "...", "type": "promoter"},
]

for data in parts_data:
    client.create_part(
        **data,
        repository_id="repo-uuid"
    )
```

## Next Steps

- [API Overview](api-overview.md) — Full API reference
- [Authentication](authentication.md) — Token management
- [Quick Start Guide](../getting-started/quick-start.md) — UI workflows
