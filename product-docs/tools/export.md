# Export Options

Export constructs, parts, and data in various formats.

## Export Formats

### GenBank (.gb)

Standard format for annotated sequences:
- Full sequence data
- All annotations
- Part references
- Metadata

Best for:
- Sharing with collaborators
- Synthesis ordering
- Archive records

### FASTA (.fasta)

Simple sequence format:
- Sequence only
- Header with name
- No annotations

Best for:
- BLAST searches
- Alignment tools
- Simple sharing

### DNA (.dna)

SnapGene-compatible format:
- Full annotations
- Visual properties
- Compatible with SnapGene viewer

### PNG Image

Export construct visualizations:
- Schematic view
- Circular map
- Presentation-ready graphics

## Exporting a Single Construct

### From Editor

1. Open the construct
2. Click **File** > **Export**
3. Select format
4. Click **Download**

### Export Options

- **Include annotations**: All or selected
- **Include parts info**: Part references
- **Sequence format**: Upper/lowercase

## Exporting Multiple Items

### Bulk Export

1. Select multiple items in repository
2. Right-click > **Export**
3. Choose format
4. Download as ZIP archive

### Export Contents

ZIP contains:
- Individual files per construct
- Manifest of contents
- Folder structure preserved

## Exporting Images

### Schematic Export

1. Open construct
2. **File** > **Export image**
3. Select **Schematic view**
4. Choose resolution
5. Download PNG

### Circular Map Export

1. Open construct (circular topology)
2. Switch to Circular map view
3. **File** > **Export image**
4. Select **Circular map**
5. Download PNG

### Image Settings

- Resolution (standard, high, print)
- Background (white, transparent)
- Labeling options

## Data Export

### Repository Export

Export repository contents:
1. Go to repository settings
2. Click **Export repository**
3. Choose what to include
4. Download archive

### Workspace Export

Contact support for full workspace exports.

## Export for Synthesis

### Preparing Files

1. Export as GenBank
2. Include all annotations
3. Run SecureDNA screen
4. Download screening certificate

### Common Requirements

Synthesis providers typically need:
- GenBank file
- SecureDNA certificate
- Order form/specifications

## API Export

Export programmatically:
- Use API endpoints
- Batch export support
- Automated workflows

See [Developer Documentation](../developer/api-overview.md).

## Best Practices

### Before Exporting

- Verify construct is complete
- Check all annotations
- Review sequence accuracy

### Format Selection

| Use Case | Recommended Format |
|----------|-------------------|
| Synthesis ordering | GenBank |
| Sharing with lab | GenBank |
| Presentations | PNG image |
| Alignment analysis | FASTA |
| SnapGene users | DNA |
| Archiving | GenBank |

### Organization

- Use consistent naming
- Include version in filename
- Keep export records

## Troubleshooting

### Export Fails

- Check construct is saved
- Verify file permissions
- Try different format

### Missing Annotations

- Verify annotations in editor
- Check export options
- Re-export with "Include all"

### Large Files

- Export subsets if needed
- Use compression
- Check download completed

## Next Steps

- [SecureDNA Scanner](secure-dna.md) — Screen before export
- [Creating Constructs](../constructs/creating-constructs.md) — Design constructs
- [BLAST Search](blast.md) — Verify exported sequences
