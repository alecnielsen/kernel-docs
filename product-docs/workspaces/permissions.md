# Permissions & Roles

Control access to your workspaces and repositories with Kernel's permission system.

## Workspace Roles

### Owner
Full control over the workspace:
- Manage all workspace settings
- Add and remove members
- Delete the workspace
- Access all repositories

### Member
Standard workspace access:
- View workspace dashboard
- Access repositories based on repository permissions
- Create new repositories
- Invite others (if allowed by settings)

## Repository Permissions

Repository permissions control who can access specific content:

### Admin
Full repository control:
- View all content
- Create, edit, delete content
- Manage repository settings
- Share with others
- Delete the repository

### Editor
Modify repository content:
- View all content
- Create new constructs, parts, files
- Edit existing content
- Delete content
- Cannot change settings or sharing

### Viewer
Read-only access:
- View all content
- Cannot create or modify
- Can copy content to their own repositories

## Permission Hierarchy

Permissions flow from workspace to repository:

```
Workspace Owner
    ↓
Repository Admin
    ↓
Repository Editor
    ↓
Repository Viewer
```

Workspace owners have admin access to all repositories by default.

## Managing Permissions

### Repository Level

1. Open the repository
2. Click **Settings** or **Share**
3. View current permissions
4. Add members:
   - Enter email or username
   - Select permission level
   - Click Add
5. Modify existing permissions:
   - Find the user
   - Change their permission level
   - Or remove access

### Workspace Level

1. Go to **Settings** > **Members**
2. View all workspace members
3. Change roles as needed
4. Remove members if necessary

## Public Repositories

Some repositories can be public:
- Accessible to all Kernel users
- Read-only by default
- Useful for sharing common resources

Public repositories include:
- Asimov Public parts
- Addgene plasmids
- UniProt sequences

## Sharing Options

### Share with Individual Users
Enter email addresses to grant access.

### Share with Workspaces
Share entire repositories with other workspaces for collaboration.

### Generate Share Link
Create a link that grants view access (if enabled).

## Best Practices

### Least Privilege
- Grant the minimum permissions needed
- Start with Viewer, upgrade as needed
- Review permissions periodically

### Repository Organization
- Group related content in repositories
- Use consistent permission patterns
- Document access policies

### Onboarding
- Create a shared parts repository for team resources
- Grant new members appropriate access
- Provide guidance on workspace organization

## Troubleshooting

### Can't Access Content
- Verify you have the correct workspace selected
- Check repository permissions with an admin
- Ensure your invitation was accepted

### Can't Edit
- Confirm you have Editor or Admin permission
- Check if the content is locked
- Contact the repository admin

### Missing Features
- Some features require Admin permissions
- Workspace owners can upgrade your access

## Next Steps

- [Creating a Workspace](creating-a-workspace.md) — Set up your team
- [Collaboration](collaboration.md) — Work together
- [Creating Repositories](../repositories/creating-repositories.md) — Organize content
