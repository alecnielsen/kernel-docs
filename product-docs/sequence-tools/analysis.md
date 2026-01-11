# Sequence Analysis

Analyze sequence properties including GC content, restriction sites, and more.

## Overview

Kernel provides tools to analyze:
- Sequence composition
- Restriction enzyme sites
- Melting temperature
- Open reading frames
- Sequence patterns

## GC Content

### View GC Content

GC percentage appears in the status bar when:
- Viewing a construct (total GC%)
- Selecting a region (selection GC%)

### GC Content Analysis

Analyze GC distribution:
- Overall percentage
- Regional variation
- GC-rich/AT-rich regions

### Why GC Content Matters

- Affects DNA stability
- Influences PCR primer design
- Impacts expression levels
- May indicate horizontal gene transfer

## Restriction Site Analysis

### Access Cut Sites Tool

1. Open a construct
2. Click **Cut sites** in the right sidebar
3. View restriction enzyme sites

### Features

- List of enzymes that cut the sequence
- Number of cut sites per enzyme
- Position of each cut site
- Visualization on sequence

### Filtering Enzymes

Filter by:
- Number of cuts (unique cutters, double cutters, etc.)
- Enzyme type
- Recognition sequence length
- Commercial availability

### Common Use Cases

- Find unique cutters for cloning
- Identify sites to avoid
- Plan restriction digests
- Verify correct assembly

## Melting Temperature

### Selection Tm

Select a region to see estimated melting temperature in the status bar.

### Tm Calculation

Kernel calculates Tm using standard methods considering:
- Sequence length
- GC content
- Salt concentration
- Primer concentration

### Applications

- Primer design
- PCR optimization
- Hybridization experiments

## Open Reading Frame Analysis

### Find ORFs

1. **View** > **Show ORFs**
2. ORFs highlight in the sequence
3. Click to see ORF details

### ORF Information

Each ORF shows:
- Start and stop positions
- Reading frame (1, 2, 3 or -1, -2, -3)
- Length in codons
- Start codon type

### Use Cases

- Identify potential coding regions
- Verify gene annotations
- Find alternative reading frames

## Sequence Search

### Within Construct

1. Click **Search** in right sidebar
2. Enter search sequence
3. Navigate between matches

### Search Options

- Case insensitive matching
- Ambiguous base support (N, R, Y, etc.)
- Reverse complement search

## Sequence Statistics

### Basic Statistics

View in Info panel:
- Total length (bp)
- GC content (%)
- Molecular weight
- Extinction coefficient

### Composition

Nucleotide frequency:
- A count and percentage
- T count and percentage
- G count and percentage
- C count and percentage

## Export Analysis

### Export Options

- Copy statistics to clipboard
- Download as text report
- Include in construct export

## Sequence Tools Integration

Combine with other tools:

| Tool | Analysis Use |
|------|--------------|
| BLAST | Find similar sequences |
| Codon Optimization | Analyze before/after |
| Simulation | Connect analysis to predictions |

## Next Steps

- [Sequence Viewer](sequence-viewer.md) — Navigate sequences
- [Codon Optimization](codon-optimization.md) — Optimize for expression
- [BLAST Search](../tools/blast.md) — Find similar sequences
