# Organization

Effectively organize your repositories for efficient work and collaboration.

## Folder Structures

### Create Folders

1. In a repository, click **New**
2. Select **Folder**
3. Name the folder
4. Click **Create**

### Nested Folders

Create hierarchies:
1. Open a folder
2. Click **New** > **Folder**
3. The new folder is nested inside

### Recommended Structures

**For Projects:**
```
Antibody-Project/
├── Heavy-Chain/
│   ├── HC-v1.gb
│   ├── HC-v2.gb
│   └── HC-optimized.gb
├── Light-Chain/
│   ├── LC-v1.gb
│   └── LC-optimized.gb
├── Constructs/
│   └── Final-Expression-System/
└── Notebooks/
    ├── Cloning-Protocol.md
    └── Expression-Results.md
```

**For Parts Libraries:**
```
Team-Parts/
├── Promoters/
│   ├── Constitutive/
│   └── Inducible/
├── CDSs/
│   ├── Reporters/
│   └── Selection-Markers/
├── Terminators/
└── Origins/
```

## Moving Content

### Drag and Drop

1. Select items in the repository view
2. Drag to a folder
3. Release to move

### Move Dialog

1. Select items
2. Right-click > **Move to...**
3. Navigate to destination
4. Click **Move**

### Across Repositories

1. Select items
2. Right-click > **Move to...**
3. Select a different repository
4. Choose location
5. Click **Move**

## Copying Content

### Within Repository

1. Select items
2. Right-click > **Duplicate**
3. Copies appear in the same location

### To Another Repository

1. Select items
2. Right-click > **Copy to...**
3. Select destination repository/folder
4. Click **Copy**

Copies are independent of originals.

## Renaming

### Single Items

1. Click the item name
2. Type new name
3. Press Enter

Or:
1. Right-click item
2. Select **Rename**
3. Enter new name
4. Confirm

### Bulk Rename

Currently, rename items individually. For large renames, consider using the API.

## Deleting Content

### Single Items

1. Select the item
2. Press **Delete** or right-click > **Delete**
3. Confirm deletion

### Multiple Items

1. Select multiple items
2. Right-click > **Delete**
3. Confirm deletion

**Warning**: Deletions are permanent.

## Favorites

Star important repositories:

1. Navigate to a repository
2. Click the star icon next to the name
3. Access favorites via **Repos** > **Favorite repositories**

## View Options

### List View

Default table view showing:
- Name
- Attributes
- Repository
- Last modified
- Modified by

### Pivot View

Group items by attribute values for analysis.

### Column Configuration

1. Click **Columns** in the repository view
2. Select which columns to display
3. Drag to reorder

## Filtering

### Filter Bar

Use dropdowns to filter by:
- **Entity types**: Constructs, parts, notebooks, etc.
- **Created by**: Specific users
- **Repositories**: Specific repositories
- **Part types**: Promoter, CDS, etc.
- **Molecule**: Associated molecules

### Quick Search

Type in the repository search bar to filter items by name.

## Best Practices

### Consistency
- Use the same structure across similar projects
- Document your organization scheme
- Train team members on conventions

### Naming
- Be descriptive: "CMV-GFP-Expression" not "Construct1"
- Use prefixes for related items
- Include version numbers

### Maintenance
- Archive completed projects to dedicated folders
- Review and clean up periodically
- Remove duplicates and outdated content

## Next Steps

- [Creating Repositories](creating-repositories.md) — Set up repositories
- [Search](search.md) — Find content quickly
- [Bulk Actions](../constructs/bulk-actions.md) — Manage multiple items
