# Codon Optimization

Optimize coding sequences for expression in specific host organisms.

## What is Codon Optimization?

Different organisms prefer different codons (three-nucleotide sequences) for the same amino acids. Codon optimization:
- Replaces rare codons with preferred synonymous codons
- Improves translation efficiency
- Can increase protein expression levels
- Maintains the same amino acid sequence

## Running Codon Optimization

### From the Construct Editor

1. Open a construct in the editor
2. Select a CDS (coding sequence) region
3. Click **CO** in the right sidebar
4. Configure optimization parameters
5. Click **Optimize**

### Optimization Parameters

- **Target organism**: Select the expression host
  - *E. coli*
  - *S. cerevisiae*
  - *CHO cells*
  - *HEK293*
  - And more
- **Optimization strategy**: Balance between codon usage and other factors

### Advanced Options

- **Avoid sequences**: Restriction sites, splice sites
- **GC content**: Target range
- **Repeat avoidance**: Minimize sequence repeats

## Viewing Results

After optimization:
- New sequence replaces the original CDS
- Original sequence preserved in history
- Compare before/after in sequence viewer

### Optimization Report

View details about the optimization:
- Codon Adaptation Index (CAI) before/after
- GC content change
- Modified codons list
- Removed problematic sequences

## Best Practices

### When to Optimize

- Expressing genes in heterologous hosts
- Low expression from native sequences
- Synthesizing genes *de novo*

### Considerations

- Rare codons sometimes have biological function
- Consider codon context, not just frequency
- Test multiple optimization strategies

### Quality Check

After optimization:
1. Verify amino acid sequence unchanged
2. Check for introduced restriction sites
3. Review GC content
4. Confirm problematic sequences removed

## Optimization History

Track optimization runs:

1. Click **Runs** in the sidebar
2. Find codon optimization runs
3. View parameters and results
4. Compare different optimizations

## API Access

Run codon optimization programmatically via the API. See [Developer Documentation](../developer/api-overview.md) for details.

## Troubleshooting

### Optimization Fails

- Verify the region is a valid CDS
- Check that start/stop codons are present
- Ensure sequence length is divisible by 3

### Unexpected Results

- Review target organism selection
- Check advanced options for conflicts
- Try different optimization strategies

## Next Steps

- [Sequence Viewer](sequence-viewer.md) — View optimized sequences
- [Sequence Analysis](analysis.md) — Analyze sequence properties
- [Simulation](../compiler-simulation/simulation.md) — Predict expression
