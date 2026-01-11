# Creating Constructs

Create new genetic constructs in Kernel using several methods.

## Create from Scratch

Start with an empty construct and build it up:

1. Click **New** > **Construct**
2. Enter a name
3. Select a destination repository
4. Choose **Empty construct**
5. Click **Create**

In the editor:
- Type or paste sequence directly
- Add parts using drag-and-drop
- Annotate features manually

## Import from File

Import existing sequences from standard file formats:

### Supported Formats
- **GenBank (.gb, .gbk)**: Full annotation support
- **FASTA (.fasta, .fa)**: Sequence only
- **DNA (.dna)**: SnapGene format

### Import Steps

1. Click **New** > **Construct**
2. Select **Import from file**
3. Upload your file
4. Review the imported sequence and annotations
5. Select a parts repository for part mapping (optional)
6. Name the construct and select destination
7. Click **Create**

### Part Mapping on Import

When importing GenBank files, Kernel can map annotations to parts:

1. During import, select a parts repository
2. Kernel matches annotations to existing parts by name
3. Review and confirm matches
4. Unmatched annotations remain as simple annotations

## Create from Template

Start from pre-built templates:

1. Click **New** > **Construct**
2. Select **From template**
3. Browse available templates:
   - Workspace templates
   - Public templates
4. Select a template
5. Customize the name and destination
6. Click **Create**

The new construct is a copy you can modify.

## Build with Parts

Assemble constructs from existing parts:

1. Create a new empty construct
2. Open **Part match** in the right sidebar
3. Search for parts
4. Drag parts into the schematic view
5. Arrange parts in order
6. Parts automatically join with appropriate seams

See [Drag and Drop Assembly](drag-and-drop.md) for detailed instructions.

## Duplicate an Existing Construct

Copy and modify an existing design:

1. Find the construct in a repository
2. Right-click and select **Duplicate**
3. Choose a destination
4. The copy opens in the editor
5. Modify as needed

## Editing Constructs

### Direct Sequence Editing

1. Click in the sequence viewer
2. Type to insert nucleotides
3. Select and delete to remove
4. Cut, copy, paste work as expected

### Insert Sequences

1. Position the cursor where you want to insert
2. Paste from clipboard, or
3. Use **Edit** > **Insert sequence**
4. Enter or paste the sequence to insert

### Replace Sequences

1. Select the region to replace
2. Type or paste the replacement sequence
3. The selection is replaced

### Delete Sequences

1. Select the region to delete
2. Press Delete or Backspace
3. The sequence is removed and the construct rejoins

## Save and Versioning

Constructs save automatically as you work. Each significant change creates a revision you can access in History.

### Manual Save
- Press **Cmd/Ctrl + S**
- Or click **File** > **Save**

### View History
1. Click **History** in the right sidebar
2. See list of revisions with timestamps
3. Click a revision to preview
4. Restore a previous version if needed

## Next Steps

- [Drag and Drop Assembly](drag-and-drop.md) — Visual parts assembly
- [Annotations](annotations.md) — Label features
- [What is a Construct?](what-is-a-construct.md) — Construct concepts
