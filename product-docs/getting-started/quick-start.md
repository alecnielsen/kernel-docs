# Quick Start Guide

Get started with Kernel in five minutes. This guide walks you through signing in, navigating your workspace, and creating your first construct.

## Sign In

1. Navigate to [kernel.asimov.com](https://kernel.asimov.com)
2. Sign in with your email
3. You'll land on your workspace dashboard

## Navigate Your Workspace

After signing in, you'll see the dashboard with:

- **Create new** buttons for Repository, Notebook, Part, and Construct
- **Latest files and repositories** showing recent work
- **Notifications** panel showing completed runs and updates

![Dashboard](../screenshots/dashboard.png)

Use the left sidebar to navigate:

| Section | Description |
|---------|-------------|
| **Home** | Dashboard with recent files and quick actions |
| **Repos** | Browse repositories, constructs, parts, and files |
| **Runs** | View simulation and optimization run history |
| **Editor** | Access the construct editor directly |
| **Tools** | BLAST search, SecureDNA scanner, and more |
| **Kernel AI** | AI assistant for genetic design |
| **Settings** | Account and workspace configuration |

## Create Your First Repository

Repositories organize your constructs, parts, and notebooks.

1. Click **New** in the top right, or click **Repository** in the Create new section
2. Enter a name for your repository
3. Add an optional description
4. Click **Create**

Your new repository appears in the Repos section.

## Create Your First Construct

Constructs are genetic designs like plasmids, vectors, or expression cassettes.

1. Click **New** > **Construct**, or use the Create new section on the dashboard
2. Choose how to start:
   - **Manual entry**: Type or paste a sequence
   - **Import file**: Upload a GenBank (.gb), DNA (.dna), or FASTA (.fasta) file
   - **From template**: Start with a pre-built template
3. Name your construct and select a destination repository
4. Click **Create**

The construct editor opens with three views:

- **Schematic**: Visual parts-based representation at the top
- **Sequence viewer**: DNA sequence with annotations
- **Circular map**: Plasmid map visualization

## Identify Parts in Your Construct

Parts are reusable genetic elements like promoters, genes, and terminators.

1. In the construct editor, click **Part match** in the right sidebar
2. Kernel analyzes your sequence and suggests matching parts from your library
3. Click a suggestion to create a part annotation at that location
4. Use the global search (**Cmd/Ctrl + K**) to find and add new parts

## Next Steps

- Learn about [Core Concepts](core-concepts.md) like workspaces, repositories, and parts
- Explore [Navigating the Interface](navigating-the-interface.md) for a detailed UI tour
- Read [Creating Constructs](../constructs/creating-constructs.md) for advanced design techniques
