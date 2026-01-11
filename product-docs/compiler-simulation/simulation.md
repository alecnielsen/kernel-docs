# Simulation

Predict gene expression behavior with Kernel's genetic simulator.

## What is Simulation?

The Simulator predicts:
- RNA polymerase flux
- Ribosome flux
- RNA concentrations
- Protein concentrations

These predictions help optimize construct design before experimental testing.

## Running Simulations

### From the Construct Editor

1. Open a construct
2. Click **Sim.** in the right sidebar
3. Configure simulation parameters
4. Click **Run Simulation**

### Simulation Parameters

- **Expression system**: Host organism
- **Copy number**: Plasmid copy number
- **Growth phase**: Exponential, stationary
- **Time course**: Simulation duration

## Understanding Results

### RNA Polymerase Flux

Measures transcription activity:
- High flux = active transcription
- Bottlenecks indicate rate-limiting regions
- Compare across constructs

### Ribosome Flux

Measures translation activity:
- Indicates protein production rate
- Identifies translation bottlenecks
- Affected by codon usage, mRNA structure

### Concentration Predictions

Predicted steady-state levels:
- mRNA concentration
- Protein concentration
- Units and scale for comparison

### Visualization

Results display as:
- Graphs over time
- Heatmaps along sequence
- Summary statistics

## Interpreting Results

### Good Design Indicators

- Smooth flux profiles
- High predicted expression
- No major bottlenecks
- Consistent with known biology

### Potential Issues

- Flux drops indicate problems
- Low expression predictions
- Imbalanced multi-gene systems
- Unusual mRNA structures

## Comparing Designs

### Side-by-Side Comparison

1. Run simulations on multiple variants
2. Open runs in **Runs** section
3. Compare predictions

### Design Iteration

1. Run initial simulation
2. Identify issues
3. Modify construct
4. Re-simulate
5. Compare improvements

## Other Prediction Types

### Signal Peptide Predictions

Predict secretion signal effectiveness:
- Signal peptide cleavage
- Secretion efficiency
- Recommended alternatives

### Antibody Developability

For antibody constructs:
- Aggregation propensity
- Stability predictions
- Immunogenicity assessment

## Run Management

### Viewing Runs

1. Click **Runs** in the sidebar
2. See all simulation runs
3. Filter by type, date, status

### Run Details

Each run shows:
- Input construct
- Parameters used
- Results and predictions
- Timestamp

### Exporting Results

- Download predictions as CSV
- Export visualizations
- Share runs with collaborators

## Best Practices

### Before Simulation

- Verify construct is complete
- Check all annotations
- Confirm expression system matches design

### Interpreting Results

- Consider predictions as estimates
- Compare relative differences
- Validate key designs experimentally

### Iterative Design

- Use simulation to guide optimization
- Test multiple variants in silico
- Focus experiments on top candidates

## Limitations

Simulations are predictive models:
- Based on known biology
- May not capture all effects
- Experimental validation recommended
- Continuously improving

## Next Steps

- [Compiler](compiler.md) — Automated design
- [Runs History](runs.md) — View all runs
- [Codon Optimization](../sequence-tools/codon-optimization.md) — Optimize sequences
