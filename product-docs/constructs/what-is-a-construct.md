# What is a Construct?

A **construct** is a designed genetic sequence in Kernel. Constructs represent plasmids, expression vectors, linear DNA fragments, or any engineered genetic element.

## Construct Components

### Sequence

The DNA sequence is the foundation of every construct. Sequences can be:
- **Circular**: Plasmids and circular vectors
- **Linear**: DNA fragments, cassettes, or linear vectors

### Parts

Parts are functional elements mapped to sequence regions:
- Promoters driving expression
- Coding sequences (genes)
- Terminators ending transcription
- Origins of replication
- Selection markers

### Annotations

Annotations label sequence features:
- Part annotations linked to part definitions
- Custom annotations for any feature
- Imported annotations from GenBank files

## Construct Views

Kernel provides three ways to visualize constructs:

### Schematic View

A symbolic representation showing parts as standardized icons:
- Parts arranged linearly
- Direction indicated by symbol orientation
- Part names labeled above
- Color-coded by part type

### Sequence Viewer

The DNA sequence displayed with:
- Nucleotide letters (A, T, G, C)
- Position markers
- Annotation tracks below the sequence
- Selection highlighting

### Circular Map

For circular constructs (plasmids):
- Parts arranged around a circle
- Size shown in the center (bp)
- Useful for visualizing plasmid organization

![Construct Editor Views](../screenshots/construct-editor-circular.png)

## Construct Properties

### Basic Information
- **Name**: Identifies the construct
- **Description**: What the construct does
- **Topology**: Circular or linear

### Metadata
- **Repository**: Where the construct is stored
- **Created/Modified**: Timestamps
- **Created by**: Author

### Attributes
Custom fields for your workflow:
- Project name
- Organism/host
- Selection marker
- Any custom properties

## Construct Groups

Construct groups link related constructs that work together. Common use cases:

### Multi-Plasmid Systems
Antibodies with separate heavy and light chain plasmids:
- HC plasmid (heavy chain)
- LC plasmid (light chain)

### Co-Transfection Sets
Multiple plasmids transfected together:
- Expression vector
- Helper plasmid
- Reporter construct

### Creating a Group
1. Select multiple constructs
2. Right-click and select **Group constructs**
3. Name the group
4. Grouped constructs appear together in searches and views

## Revisions

Kernel tracks construct history:
- Every save creates a revision
- View revision history in the History panel
- Compare changes between versions
- Revert to previous versions if needed

## Next Steps

- [Creating Constructs](creating-constructs.md) — Build new constructs
- [Drag and Drop Assembly](drag-and-drop.md) — Visual construct design
- [Annotations](annotations.md) — Label sequence features
