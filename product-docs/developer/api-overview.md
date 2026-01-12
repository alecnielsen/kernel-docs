# API Overview

Access Kernel programmatically through our REST and GraphQL APIs.

## API Resources

Kernel provides multiple API interfaces:

### REST API

OpenAPI-compliant REST endpoints for:
- CRUD operations on constructs, parts, repositories
- File upload/download
- Search and filtering
- Run management

**Documentation**: [https://kv2.dev.asimov.io/docs](https://kv2.dev.asimov.io/docs)

### GraphQL API

Flexible GraphQL interface for:
- Complex queries
- Relationship traversal
- Efficient data fetching

**Endpoint**: `https://kv2.dev.asimov.io/graphql`

### Python SDK

Official Python client library:
- Simplified API access
- Type hints
- Common operations

## Getting Started

### 1. Create API Token

1. Go to **Settings** > **Security** > **API Tokens**
2. Click **Create Token**
3. Name and configure the token
4. Copy the token (shown once)

### 2. Test Connection

```bash
curl -H "Authorization: Bearer YOUR_TOKEN" \
  https://kv2.dev.asimov.io/api/v1/me
```

### 3. Explore Documentation

Visit the Swagger UI at `/docs` to explore endpoints interactively.

## Python SDK

### Installation

```bash
pip install kernel-sdk
```

### Basic Usage

```python
from kernel import KernelClient

# Initialize client
client = KernelClient(token="YOUR_TOKEN")

# Get current user
me = client.get_me()
print(f"Logged in as: {me.name}")

# List workspaces
workspaces = client.list_workspaces()
for ws in workspaces:
    print(f"- {ws.name}")

# Get constructs
constructs = client.list_constructs(workspace_id="...")
```

### Common Operations

```python
# Create a construct
construct = client.create_construct(
    name="My Construct",
    sequence="ATGCATGC...",
    repository_id="..."
)

# Get construct details
construct = client.get_construct(construct_id="...")
print(f"Length: {len(construct.sequence)} bp")

# Update construct
client.update_construct(
    construct_id="...",
    name="Updated Name"
)

# Export as GenBank
genbank = client.export_construct(
    construct_id="...",
    format="genbank"
)
```

## Authentication

### Bearer Token

Include token in Authorization header:

```
Authorization: Bearer YOUR_TOKEN
```

### Token Scopes

Tokens can have limited scopes:
- `read`: Read-only access
- `write`: Create and modify
- `admin`: Full access

### Token Security

- Store tokens securely
- Use environment variables
- Rotate tokens regularly
- Revoke unused tokens

## Rate Limits

API requests are rate limited:
- 1000 requests per minute
- Burst allowance for short peaks
- Rate limit headers in responses

## Error Handling

### HTTP Status Codes

| Code | Meaning |
|------|---------|
| 200 | Success |
| 201 | Created |
| 400 | Bad request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not found |
| 429 | Rate limited |
| 500 | Server error |

### Error Response Format

```json
{
  "error": {
    "code": "INVALID_REQUEST",
    "message": "Detailed error message"
  }
}
```

## Webhooks

*Coming soon*

Receive notifications for events:
- Construct created/updated
- Run completed
- Repository changes

## Best Practices

### Efficiency

- Use pagination for large lists
- Request only needed fields (GraphQL)
- Cache responses where appropriate

### Reliability

- Handle rate limits gracefully
- Implement retry logic
- Log API calls for debugging

### Security

- Never commit tokens to code
- Use minimal required scopes
- Audit token usage

## Support

### API Issues

- Check status at status.asimov.com
- Review documentation
- Contact api-support@asimov.com

### SDK Issues

- GitHub issues for SDK bugs
- Documentation feedback welcome

## Next Steps

- [Authentication](authentication.md) — Detailed auth guide
- [Common Operations](common-operations.md) — Code examples
- [Account Settings](../settings/account-workspace.md) — Create API tokens
