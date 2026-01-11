# Annotations

Annotations label features and regions within your construct sequence.

## What Are Annotations?

Annotations are simple labels that mark specific sequence regions. They document features within your construct but are not designed for reuse across designs. Each annotation has:
- **Name**: Feature identifier
- **Type**: Category label (CDS, misc_feature, etc.)
- **Location**: Start and end positions
- **Direction**: Forward or reverse strand
- **Additional properties**: Color, notes, qualifiers

## Annotations vs. Parts

**Simple annotations** are lightweight labels:
- Exist only within one construct
- Good for documenting features from imported files
- Not searchable as standalone items
- Not intended for reuse

**Parts** are reusable genetic elements:
- Have their own file and identity
- Searchable across your workspace
- Designed for reuse in multiple constructs
- Contain rich metadata

If you have a genetic element you want to reuse (a promoter, gene, terminator, etc.), create it as a part rather than just annotating it. See [Creating Parts](../parts/creating-parts.md).

## Creating Annotations

### From Selection

1. In the sequence viewer, select a region by clicking and dragging
2. Right-click the selection
3. Select **Create annotation**
4. Enter:
   - Name
   - Type (CDS, promoter, misc_feature, etc.)
   - Strand direction
5. Click **Create**

### From Parts

When you add a part to a construct:
- A part annotation is automatically created
- Links the sequence region to the part definition

### Import with File

GenBank files include annotations:
- Annotations import automatically
- Review and edit imported annotations
- Optionally link to existing parts

## Editing Annotations

### Change Properties

1. Click an annotation in the sequence viewer
2. The annotation details panel opens
3. Edit name, type, or other properties
4. Changes save automatically

### Resize Annotation

1. Select the annotation
2. Drag the edges to resize
3. Or edit start/end positions in the properties panel

### Move Annotation

1. Select the annotation
2. Drag to a new location
3. Or update the position values

### Delete Annotation

1. Select the annotation
2. Press **Delete** or right-click and select **Delete annotation**

## Annotation Visualization

### Sequence Viewer

Annotations appear as:
- Colored bars below the sequence
- Labels showing annotation name
- Arrows indicating direction

### Schematic View

Part annotations show as:
- Symbols in the schematic
- Names angled above
- Color-coded by type

### Circular Map

On circular constructs:
- Annotations display around the circle
- Color and labels match other views

## Annotation Types

Common annotation types:

| Type | Description |
|------|-------------|
| CDS | Coding sequence (gene) |
| promoter | Transcription promoter |
| terminator | Transcription terminator |
| rep_origin | Replication origin |
| misc_feature | General feature |
| primer_bind | Primer binding site |
| protein_bind | Protein binding site |
| regulatory | Regulatory element |

## Managing Multiple Annotations

### Overlapping Annotations

Annotations can overlap:
- Common for nested features
- Displayed in stacked tracks
- Each maintains independent properties

### Bulk Operations

Select multiple annotations:
- **Shift-click**: Select range
- **Cmd/Ctrl-click**: Add to selection
- Apply changes to all selected

### Hide/Show Annotations

Control annotation visibility:
1. Click **View** menu
2. Select **Annotation visibility**
3. Toggle types on/off
4. Simplify the view for complex constructs

## Linking to Parts

### Convert Annotation to Part

1. Select a simple annotation
2. Right-click and select **Create part from annotation**
3. Fill in part details
4. The annotation becomes a part annotation

### Link Existing Part

1. Select an annotation
2. In properties, click **Link to part**
3. Search and select a part
4. The annotation references that part

## Best Practices

### Naming
- Use clear, descriptive names
- Follow conventions (e.g., GenBank standard names)
- Be consistent across constructs

### Organization
- Annotate all functional regions
- Use appropriate types
- Include notes for complex features

### Maintenance
- Update annotations when sequences change
- Link annotations to parts for reusability
- Review imported annotations for accuracy

## Next Steps

- [What is a Construct?](what-is-a-construct.md) — Construct overview
- [Creating Parts](../parts/creating-parts.md) — Build reusable parts from annotations
- [Sequence Viewer](../sequence-tools/sequence-viewer.md) — Working with sequences
