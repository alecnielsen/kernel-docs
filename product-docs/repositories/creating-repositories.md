# Creating Repositories

Repositories organize your constructs, parts, notebooks, and files into logical collections.

## Create a Repository

1. Click **New** > **Repository** in the header
2. Or click **Repository** in the dashboard Create new section
3. Enter repository details:
   - **Name**: Descriptive identifier
   - **Description**: Purpose and contents
4. Click **Create**

The new repository appears in your Repos list.

## Repository Contents

Repositories can contain:

- **Constructs**: Plasmids, vectors, genetic designs
- **Parts**: Reusable genetic elements
- **Notebooks**: Lab notes and documentation
- **Folders**: Organize content hierarchically
- **Files**: Supporting documents

## Repository Settings

Access settings by clicking **Settings** in a repository:

### General
- Name and description
- Repository visibility

### Sharing
- Add collaborators
- Set permission levels
- Share with workspaces

### Advanced
- Delete repository (Admin only)

## Repository Types

### Project Repositories
Contain all content for a specific project:
- Related constructs
- Project-specific parts
- Notebooks with protocols and results

### Parts Libraries
Dedicated to reusable parts:
- Organized by part type
- Shared across the workspace
- Well-documented with metadata

### Template Repositories
Store starting points for new designs:
- Backbone templates
- Common configurations
- Standard protocols

## Organizing with Folders

### Create Folders

1. In a repository, click **New** > **Folder**
2. Name the folder
3. Click **Create**

### Folder Structure Examples

**By Function:**
```
Project-Name/
├── Constructs/
├── Parts/
│   ├── Promoters/
│   ├── CDSs/
│   └── Terminators/
└── Notebooks/
```

**By Stage:**
```
Project-Name/
├── Design/
├── Testing/
├── Production/
└── Archive/
```

### Move Items to Folders

1. Select items in the repository
2. Drag to the target folder
3. Or right-click and select **Move to...**

## Importing Content

### From Files

1. In the repository, click **New**
2. Select the content type (Construct, Part, etc.)
3. Choose **Import from file**
4. Upload your files

### From Other Repositories

1. Find content in another repository
2. Right-click and select **Copy to...**
3. Choose the destination repository

## Best Practices

### Naming Conventions
- Use consistent prefixes
- Include project codes
- Add version identifiers when relevant

### Documentation
- Write clear descriptions
- Keep README notebooks
- Document organization schemes

### Maintenance
- Archive completed projects
- Remove outdated content
- Review permissions regularly

## Next Steps

- [Organization](organization.md) — Structure your repositories
- [Search](search.md) — Find content
- [Permissions & Roles](../workspaces/permissions.md) — Control access
