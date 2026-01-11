# Compiler

The Compiler automates plasmid design for antibody and protein expression.

## What is the Compiler?

The Compiler generates complete expression constructs from amino acid sequences. Given a protein sequence, it automatically:

- Optimizes codons for the target host
- Predicts and adds signal peptides
- Selects appropriate vector backbones
- Assembles all required genetic elements
- Generates ready-to-order plasmid designs

## Supported Molecule Types

### Monoclonal Antibodies (mAbs)

Standard antibody formats:
- Heavy chain + Light chain
- IgG, IgA, IgM formats
- Different isotype variants

### Bispecific Antibodies

Antibodies targeting two antigens:
- Knob-in-hole formats
- CrossMab designs
- Common bispecific architectures

### Fusion Proteins

Protein fusions:
- Fc-fusions
- Albumin fusions
- Custom linker options

### Multispecific Molecules

Complex formats:
- Trispecifics
- Multi-domain proteins
- Custom architectures

## Running the Compiler

### Input Requirements

1. **Amino acid sequences**: Protein sequences to express
2. **Format selection**: Molecule architecture
3. **Expression system**: Target host (CHO, HEK293, etc.)

### Workflow

1. Create a new molecule or select existing
2. Enter amino acid sequences
3. Select molecule format
4. Configure expression parameters
5. Run the Compiler
6. Review generated constructs

### Configuration Options

- **Codon optimization**: Target organism preferences
- **Signal peptide**: Auto-predict or specify
- **Vector template**: Select backbone
- **Regulatory elements**: Promoter, terminator choices

## Compiler Components

### Codon Optimization

The Compiler includes Asimov's proprietary codon optimizer:
- Optimized for mammalian expression
- Avoids problematic sequences
- Maintains optimal GC content

### Signal Peptide Prediction

Automatic signal peptide selection:
- Predicts optimal secretion signals
- Based on sequence properties
- Uses validated peptide library

### Vector Templates

Pre-configured expression vectors:
- Optimized for specific hosts
- Include selection markers
- Ready for manufacturing

### Expert Rules

Built-in design rules from:
- Literature best practices
- Asimov internal expertise
- Validated configurations

## Reviewing Output

### Generated Constructs

The Compiler creates:
- Complete plasmid sequences
- Full annotations
- Linked parts
- Ready for simulation

### Construct Groups

Multi-chain molecules generate grouped constructs:
- HC plasmid
- LC plasmid
- Linked as a molecule

### Quality Checks

Review automated checks:
- Sequence validation
- Reading frame verification
- Signal peptide placement
- Restriction site analysis

## Templates

### Preferred Templates

Mark templates as preferred:
1. Open template construct
2. In Info panel, mark as preferred
3. Compiler prioritizes this template

### Custom Templates

Create custom vector templates:
1. Design your backbone
2. Add template markers
3. Save as template
4. Use in Compiler runs

## Best Practices

### Input Quality

- Verify amino acid sequences
- Check for unusual residues
- Confirm sequence boundaries

### Format Selection

- Choose the simplest format that meets needs
- Consider manufacturing requirements
- Account for downstream applications

### Review Output

- Check generated sequences
- Verify annotations
- Run simulations on output
- Confirm vector elements

## Next Steps

- [Simulation](simulation.md) — Predict expression
- [Runs History](runs.md) — View past runs
- [Creating Constructs](../constructs/creating-constructs.md) — Manual design
