# SecureDNA Scanner

Screen sequences for biosecurity concerns using the SecureDNA service.

## What is SecureDNA?

SecureDNA is a biosecurity screening system that:
- Checks sequences against hazard databases
- Identifies potentially dangerous sequences
- Supports responsible genetic engineering
- Required by many synthesis providers

## Running a Screen

### From Tools

1. Click **Tools** in the sidebar
2. Select **SecureDNA Scanner**
3. Enter or paste sequence
4. Click **Screen**

### From Construct Editor

1. Open a construct
2. Click the SecureDNA icon in the toolbar
3. Screen runs automatically on the full construct

### Batch Screening

Screen multiple constructs:
1. Select constructs in repository
2. Right-click > **Screen with SecureDNA**
3. View results for all

## Understanding Results

### Clear Result

Your sequence passed screening:
- No hazardous sequences detected
- Safe to proceed with synthesis
- Keep results for records

### Flagged Result

Potential concern detected:
- Review the flagged region
- Understand why it was flagged
- May need modification or justification

### Result Categories

| Category | Meaning |
|----------|---------|
| Pass | No concerns |
| Flag | Requires review |
| Block | Cannot proceed |

## Working with Flagged Sequences

### Review Details

1. Click on flagged result
2. See specific concern
3. View flagged sequence region

### Common Causes

- Toxin-encoding sequences
- Pathogen genes
- Virulence factors
- Dual-use research concern genes

### Resolution Options

1. **Modify sequence**: Remove or alter problematic region
2. **Provide justification**: Document legitimate research purpose
3. **Contact support**: Get guidance on compliance

## Synthesis Provider Requirements

### Pre-Order Screening

Many providers require SecureDNA screening:
1. Screen your construct
2. Download screening certificate
3. Include with synthesis order

### Export Certificate

1. View screening result
2. Click **Download Certificate**
3. PDF includes:
   - Sequence identifier
   - Screening date
   - Result summary
   - SecureDNA verification

## Best Practices

### Regular Screening

- Screen all constructs before synthesis
- Re-screen after modifications
- Keep screening records

### Design Considerations

- Be aware of hazardous sequences
- Consider alternatives for flagged regions
- Document research justification

### Compliance

- Follow institutional biosafety guidelines
- Maintain screening documentation
- Report concerns appropriately

## Integration

### Automatic Screening

Enable automatic screening:
1. Go to workspace settings
2. Enable SecureDNA on construct creation
3. All new constructs screened automatically

### API Access

Screen programmatically via API for:
- Batch processing
- Pipeline integration
- Automated workflows

## Troubleshooting

### Screening Fails

- Check sequence validity
- Verify internet connection
- Try again later

### Unexpected Flag

- Review the specific concern
- Check for sequence accuracy
- Contact support if unclear

## Resources

- [SecureDNA website](https://securedna.org)
- Institutional Biosafety Committee
- Kernel support for screening questions

## Next Steps

- [BLAST Search](blast.md) — Sequence similarity
- [Export Options](export.md) — Export with certificates
- [Creating Constructs](../constructs/creating-constructs.md) — Design safe constructs
