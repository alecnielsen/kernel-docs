# BLAST Search

Find similar sequences across your workspace and public databases.

## What is BLAST?

BLAST (Basic Local Alignment Search Tool) finds sequences similar to your query. Use it to:
- Find related constructs or parts
- Identify homologs
- Check for unintended sequence matches
- Verify construct identity

## Running BLAST

### Access BLAST

1. Press **Cmd/Ctrl + K** to open global search
2. Enter your query sequence or search term
3. Use the BLAST search option to find similar sequences

Or from the construct editor:
1. Select a sequence region
2. Right-click > **BLAST selection**

### Input Query

Enter your query sequence:
- Paste nucleotide sequence
- Select from open construct
- Enter accession number

### Configure Search

**Search Database:**
- Workspace constructs
- Workspace parts
- Public databases

**Search Type:**
- blastn (nucleotide vs. nucleotide)
- blastx (translated nucleotide vs. protein)
- tblastn (protein vs. translated nucleotide)

**Parameters:**
- E-value threshold
- Word size
- Gap penalties

## Understanding Results

### Results Table

| Column | Description |
|--------|-------------|
| Hit | Matching sequence name |
| Score | Alignment score |
| E-value | Statistical significance |
| Identity | Percent identical |
| Coverage | Query coverage |
| Location | Repository and position |

### Alignment View

Click a result to see:
- Sequence alignment
- Matching regions
- Gaps and mismatches

### E-value Interpretation

| E-value | Meaning |
|---------|---------|
| < 1e-50 | Very strong match |
| 1e-50 to 1e-10 | Strong match |
| 1e-10 to 1e-5 | Moderate match |
| > 1e-5 | Weak match (may be random) |

## Using Results

### Navigate to Hit

Click a result to open the matching construct or part in a new tab.

### Add to Construct

1. Select a hit
2. Click **Add to construct**
3. Choose destination construct
4. Insert the matching sequence

### Export Results

- Download as CSV
- Copy alignment to clipboard
- Save search for reference

## Search Strategies

### Find Similar Parts

1. Enter your part sequence
2. Search workspace parts
3. Find existing similar parts
4. Avoid redundant creation

### Verify Constructs

1. BLAST your construct
2. Check expected hits appear
3. Look for unexpected matches
4. Verify correct assembly

### Find Homologs

1. Enter gene sequence
2. Search public databases
3. Identify orthologs/paralogs
4. Guide phylogenetic analysis

## Best Practices

### Query Selection

- Use representative region
- Avoid repetitive sequences
- Include enough context (>50 bp)

### Database Selection

- Start with workspace search
- Expand to public if needed
- Use appropriate search type

### Result Analysis

- Check E-values for significance
- Verify alignments make sense
- Consider biological context

## Troubleshooting

### No Results

- Check query sequence validity
- Broaden E-value threshold
- Search additional databases

### Too Many Results

- Tighten E-value threshold
- Use longer query sequence
- Filter results by coverage

### Slow Search

- Large databases take time
- Consider shorter query
- Use more specific databases

## Next Steps

- [SecureDNA Scanner](secure-dna.md) — Biosecurity screening
- [Search](../repositories/search.md) — Text-based search
- [Sequence Analysis](../sequence-tools/analysis.md) — Other analysis tools
