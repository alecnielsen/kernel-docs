# FAQ

Frequently asked questions about Kernel.

## General

### What is Kernel?

Kernel is a genetic design platform for engineering biology. It combines sequence design tools, team collaboration features, and workflow automation to accelerate biotechnology development.

### Who is Kernel for?

Kernel is designed for:
- Molecular biologists designing constructs
- Antibody engineers
- Synthetic biologists
- Research teams collaborating on genetic projects
- Bioinformaticians managing sequence data

### How do I get started?

1. Sign up at [kernel.asimov.com](https://kernel.asimov.com)
2. Join or create a workspace
3. Follow the [Quick Start Guide](../getting-started/quick-start.md)

## Account & Access

### How do I reset my password?

1. Go to the login page
2. Click "Forgot password"
3. Enter your email address
4. Follow the reset link sent to your email

### Can I belong to multiple workspaces?

Yes. You can be a member of multiple workspaces and switch between them using the workspace selector in the header.

### How do I invite team members?

1. Go to **Settings** > **Members**
2. Click **Invite**
3. Enter email addresses
4. Select their role
5. Send invitations

## Constructs & Parts

### What file formats can I import?

Kernel supports:
- GenBank (.gb, .gbk)
- FASTA (.fasta, .fa)
- DNA (.dna) - SnapGene format

### What file formats can I export?

- GenBank (.gb)
- FASTA (.fasta)
- DNA (.dna)
- PNG images (schematic, circular map)

### What's the difference between a part and an annotation?

**Parts** are reusable genetic elements stored in your library. They have defined properties and can be used across multiple constructs.

**Annotations** are labels on sequence regions. They can be standalone or linked to part definitions.

### How do I create a construct from parts?

1. Create a new construct
2. Open Part match in the right sidebar
3. Search for parts
4. Drag parts into the schematic view
5. Arrange as needed

See [Drag and Drop Assembly](../constructs/drag-and-drop.md).

## Collaboration

### How do I share a repository?

1. Open the repository
2. Click **Share**
3. Add users or workspaces
4. Set permission levels
5. Click **Share**

### What are the permission levels?

- **Admin**: Full control including settings
- **Editor**: Can create and modify content
- **Viewer**: Read-only access

### Can I share with people outside my organization?

Yes. Share repositories with any Kernel user by email, or share with other workspaces.

## Tools & Features

### What is codon optimization?

Codon optimization replaces rare codons with more common synonymous codons for your target expression host. This can improve protein expression while maintaining the same amino acid sequence.

### What is the Compiler?

The Compiler automatically designs expression constructs from antibody amino acid sequences. It handles codon optimization, signal peptide selection, and vector assembly.

### What is SecureDNA?

SecureDNA is a biosecurity screening service that checks sequences for potentially hazardous content. It's often required by synthesis providers.

### What simulations can Kernel run?

Kernel's Simulator predicts:
- RNA polymerase flux
- Ribosome flux
- RNA concentrations
- Protein concentrations

## Technical

### Is there an API?

Yes. Kernel provides REST and GraphQL APIs, plus a Python SDK. See [API Overview](../developer/api-overview.md).

### What browsers are supported?

Kernel works best in:
- Chrome (recommended)
- Firefox
- Safari
- Edge

### Is my data secure?

Yes. Kernel uses industry-standard security:
- Encrypted data in transit and at rest
- Role-based access control
- Regular security audits

## Troubleshooting

### Why can't I edit a construct?

Possible reasons:
- You have Viewer permission (need Editor or Admin)
- The construct is locked
- You're viewing a public repository

Contact the repository admin for access.

### Why is my search not finding results?

Try:
- Check spelling
- Use fewer search terms
- Remove filters
- Search in "All repositories" instead of "This folder"

### Why did my simulation fail?

Common causes:
- Invalid sequence format
- Missing annotations
- Incomplete construct
- Check the error message for details

## Support

### How do I get help?

- Check this documentation
- Use [Kernel AI](../kernel-ai/using-kernel-ai.md) for guidance
- Email [kernel-support@asimov.com](mailto:kernel-support@asimov.com)

### How do I report a bug?

Email kernel-support@asimov.com with:
- What you were trying to do
- What happened
- Steps to reproduce
- Screenshots if helpful

### How do I request a feature?

Email kernel-support@asimov.com with your feature request. We review all suggestions.
