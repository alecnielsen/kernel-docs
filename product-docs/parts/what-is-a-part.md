# What is a Part?

A **part** is a reusable genetic element with a defined biological function. Parts are the building blocks of genetic constructs in Kernel.

## Part Types

Parts are categorized by their biological function:

### Regulatory Elements

| Type | Function | Example |
|------|----------|---------|
| **Promoter** | Drives transcription initiation | CMV promoter, T7 promoter |
| **5' UTR** | Affects translation efficiency | Kozak sequence |
| **3' UTR** | Influences mRNA stability | SV40 poly(A) signal |
| **Terminator** | Ends transcription | BGH terminator |
| **Enhancer** | Increases transcription | CMV enhancer |
| **Insulator** | Blocks regulatory interference | CTCF-binding insulator |

### Coding Sequences

| Type | Function | Example |
|------|----------|---------|
| **CDS** | Protein coding sequence | GFP, lacZ, antibody chains |
| **Signal peptide** | Targets protein localization | IgK signal peptide |
| **Tag** | Protein purification/detection | His-tag, FLAG-tag |

### Structural Elements

| Type | Function | Example |
|------|----------|---------|
| **Origin** | DNA replication start | pUC origin, ColE1 |
| **Selectable marker** | Selection in host cells | Ampicillin resistance |
| **Linker** | Connects protein domains | (G4S)3 linker |
| **Seam** | Junction between parts | Standard seam sequences |

### RNA Elements

| Type | Function | Example |
|------|----------|---------|
| **RBS** | Ribosome binding site | Shine-Dalgarno sequence |
| **Ribozyme** | RNA with catalytic activity | Hammerhead ribozyme |
| **RNA regulatory** | RNA-based regulation | Toehold switch |

## Part Properties

Each part has:

### Required Properties
- **Name**: Unique identifier
- **Type**: Functional classification
- **Sequence**: DNA sequence

### Optional Properties
- **Description**: What the part does
- **Organism**: Source organism
- **Source**: Where the part came from (paper, database)
- **Attributes**: Custom metadata fields

## Parts vs. Annotations

**Parts** are reusable genetic elements with their own identity. Each part:
- Has its own file in your repository
- Contains rich metadata (type, organism, source, description)
- Is searchable across your workspace
- Can be referenced by multiple constructs
- Is designed for reuse across designs

**Annotations** are simple labels that mark regions within a sequence. They:
- Exist only within the construct they belong to
- Label sequence features for documentation
- Are not searchable as standalone items
- Are not designed for reuse

Use parts for genetic elements you plan to reuse (promoters, genes, terminators). Use simple annotations for one-off labels or features imported from GenBank files that you don't need to track separately.

## Part Visualization

In the construct editor, parts appear as:

- **Schematic symbols**: Standardized icons showing part type and direction
- **Colored regions**: In the sequence viewer, parts are highlighted
- **Labels**: Part names appear in the schematic view

## Next Steps

- [Creating Parts](creating-parts.md) — Add parts to your library
- [Part Library](part-library.md) — Access public part collections
- [Creating Constructs](../constructs/creating-constructs.md) — Use parts in designs
