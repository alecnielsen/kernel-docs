# Inventory Overview

Track physical samples and link them to your digital designs.

## What is Inventory?

The Inventory system connects:
- Physical samples (DNA, plasmids, strains)
- Storage locations (freezers, boxes, wells)
- Digital constructs and parts

## Key Concepts

### Items

Inventory items represent physical samples:
- Linked to a construct or part
- Have a storage location
- Include quantity and status

### Locations

Hierarchical storage structure:
- **Freezers**: Top-level storage units
- **Boxes**: Containers within freezers
- **Wells**: Specific positions in boxes

### Linking to Constructs

Each inventory item can link to:
- A construct in your repository
- A part definition
- Associated metadata

## Adding Inventory Items

### From a Construct

1. Open a construct
2. In Info panel, click **Add to inventory**
3. Enter item details:
   - Quantity
   - Location
   - Notes
4. Click **Save**

### Manual Entry

1. Go to Inventory section
2. Click **Add item**
3. Fill in details:
   - Name
   - Type (DNA, plasmid, strain)
   - Location
   - Linked construct (optional)
4. Click **Create**

## Managing Locations

### Create a Freezer

1. In Inventory, click **Locations**
2. Click **Add freezer**
3. Enter name and details
4. Click **Create**

### Add Boxes

1. Open a freezer
2. Click **Add box**
3. Enter box name
4. Specify grid size (rows × columns)
5. Click **Create**

### Assign Wells

1. Open a box
2. Click empty well
3. Assign inventory item
4. Or mark as empty/reserved

## Finding Items

### Search Inventory

1. Use the search bar in Inventory
2. Search by:
   - Item name
   - Location
   - Linked construct
   - Notes

### Filter Options

Filter by:
- Item type
- Location
- Status
- Date added

## Item Details

Each item shows:
- Name and type
- Location path (Freezer > Box > Well)
- Linked construct/part
- Quantity and units
- Creation date
- Notes

## Tracking Usage

### Update Quantity

1. Open item details
2. Click **Update quantity**
3. Enter new quantity
4. Add note about usage

### Item History

View item history:
- Quantity changes
- Location moves
- Notes and updates

## Best Practices

### Labeling

- Use consistent naming
- Include construct name in item name
- Add prep date to notes

### Organization

- Group related items
- Use logical box arrangements
- Document storage schemes

### Maintenance

- Regularly audit inventory
- Remove depleted items
- Update locations when moving

## Integration

### Linking Workflow

1. Design construct in Kernel
2. Order synthesis/cloning
3. Receive physical sample
4. Add to inventory linked to construct

### Traceability

Track from design to sample:
- Construct revision
- Inventory item
- Experimental use

## Next Steps

- [Creating Constructs](../constructs/creating-constructs.md) — Design before making
- [Organization](../repositories/organization.md) — Keep designs organized
- [Search](../repositories/search.md) — Find linked constructs
