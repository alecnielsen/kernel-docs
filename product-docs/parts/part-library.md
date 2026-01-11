# Part Library

Access curated genetic parts from public collections and your workspace.

## Public Repositories

Kernel provides access to several public repositories:

### Asimov Public

A curated repository of genetic parts maintained by Asimov, including:
- Promoters for various expression systems
- Common coding sequences (reporters, selection markers)
- Terminators and regulatory elements
- Optimized sequences for mammalian expression

To access:
1. Go to **Repos** in the sidebar
2. Click **Public repositories**
3. Select **Asimov Public**

### Addgene

A public repository of plasmid sequences from Addgene:
- Thousands of deposited plasmids
- Full sequence and annotation data
- Links to original publications

### UniProt Swiss-Prot

A public repository of protein sequences from UniProt:
- Curated protein information
- Functional annotations
- Cross-references to literature

## Finding Parts

### Part Match

When editing a construct, Part match suggests existing parts that match regions of your sequence:

1. Click **Part match** in the right sidebar
2. Kernel analyzes your construct's sequence
3. Matching parts from your accessible repositories appear as suggestions
4. Click a suggestion to annotate that region as a part

### Global Search

Search across all accessible parts:

1. Press **Cmd/Ctrl + K** to open search
2. Type your query
3. Filter results to show only Parts
4. Click to open or add to a construct

### Browse by Repository

1. Go to **Repos** > **All parts**
2. Filter by repository, type, or creator
3. Sort by name, date modified, or other columns

## Using Public Parts

### Copy to Your Repository

To customize a public part:

1. Find the part in a public collection
2. Right-click and select **Copy**
3. Choose your destination repository
4. The copied part is now yours to edit

### Reference Directly

You can use public parts directly in constructs without copying:

1. Drag the part from Part match into your construct
2. The construct references the public part
3. Updates to the public part reflect in your construct

## Sharing Your Parts

### Share Within Workspace

Parts in workspace repositories are automatically accessible to workspace members based on repository permissions.

### Share Across Workspaces

1. Open the repository containing the part
2. Click **Share**
3. Add the target workspace or user
4. Set permission level (Viewer, Editor, Admin)

## Part Collections

Organize parts into collections for easy access:

### Create a Parts Repository

1. Click **New** > **Repository**
2. Name it (e.g., "Team Parts Library")
3. Add a description
4. Move or copy commonly used parts here

### Folder Organization

Within a parts repository:
- **Promoters/** — All promoter parts
- **CDSs/** — Coding sequences
- **Terminators/** — Terminator elements
- **By Project/** — Project-specific parts

## Best Practices

### Curating Your Library

- Verify sequences before adding to shared libraries
- Include complete metadata (source, organism, function)
- Use consistent naming conventions
- Document modifications from original sources

### Version Control

- Keep original versions of public parts
- Create copies before making modifications
- Note changes in the description field

## Next Steps

- [What is a Part?](what-is-a-part.md) — Understanding part types
- [Creating Parts](creating-parts.md) — Add your own parts
- [Creating Constructs](../constructs/creating-constructs.md) — Use parts in designs
