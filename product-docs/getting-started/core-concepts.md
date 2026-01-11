# Core Concepts

Understanding Kernel's core concepts helps you organize your work and collaborate effectively.

## Workspaces

A **workspace** is a shared environment where teams collaborate on genetic design projects. Each workspace has:

- **Members**: Users with access to the workspace
- **Repositories**: Collections of constructs, parts, and notebooks
- **Settings**: Configuration for the workspace

You can belong to multiple workspaces and switch between them using the workspace selector in the header.

### Public Workspaces

Kernel provides access to public workspaces with curated content:

- **Asimov Public**: Curated genetic parts from Asimov
- **Uniprot Swiss-Prot**: Protein sequences and annotations
- **Addgene**: Plasmid repository

## Repositories

A **repository** is a container for organizing related constructs, parts, notebooks, and files. Think of it like a project folder.

Repositories support:

- **Folders**: Organize content hierarchically
- **Sharing**: Control who can view or edit
- **Permissions**: Admin, Editor, or Viewer roles

## Constructs

A **construct** is a designed genetic sequence, typically a plasmid or expression vector. Constructs are built from parts and can include:

- DNA sequences
- Annotations marking features and regions
- Parts mapped to sequence regions
- Metadata like name, description, and attributes

### Construct Groups

A **construct group** links related constructs that function together. For example, an antibody expression system might include:

- Heavy chain plasmid
- Light chain plasmid

Grouping these constructs keeps them organized and indicates they're meant to be used together.

## Parts

A **part** is a reusable genetic element with a defined function. Parts have:

- **Type**: Promoter, CDS, terminator, origin, etc.
- **Sequence**: The DNA sequence
- **Attributes**: Metadata like organism, function, source

Common part types:

| Type | Function |
|------|----------|
| Promoter | Drives transcription |
| 5' UTR | Untranslated region affecting translation |
| CDS | Coding sequence (gene) |
| 3' UTR | Untranslated region for stability |
| Terminator | Ends transcription |
| Origin | Replication origin |
| Selectable marker | Antibiotic resistance or selection |

## Molecules

A **molecule** is a higher-level entity representing a protein or complex that one or more constructs encode. Molecules are particularly useful for:

- Antibodies (linking heavy and light chain constructs)
- Multi-subunit proteins
- Protein complexes

## Notebooks

**Notebooks** are electronic lab notebook (ELN) entries for documenting experiments, protocols, and notes. Notebooks can link to constructs and parts for traceability.

## Sequences

Sequences in Kernel are DNA sequences with annotations. Key concepts:

- **Annotations**: Named regions marking features (promoters, genes, etc.)
- **Parts mapping**: Linking sequence regions to part definitions
- **Topology**: Linear or circular (plasmids)

## Next Steps

- [Navigating the Interface](navigating-the-interface.md) — Learn the UI layout
- [Creating Constructs](../constructs/creating-constructs.md) — Build your first design
- [Parts Library](../parts/part-library.md) — Find reusable parts
