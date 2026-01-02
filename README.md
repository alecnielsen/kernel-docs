# Kernel Documentation

User documentation for [Kernel](https://kernel.asimov.com), Asimov's genetic design platform.

**Live docs:** https://docs.kernel.asimov.com

## About Kernel

Kernel is a collaborative platform for designing genetic constructs, including plasmids, vectors, and antibody expression systems. It provides tools for sequence visualization, codon optimization, simulation, and team collaboration.

## Repository Structure

```
product-docs/           # Documentation source (GitBook markdown)
├── getting-started/    # Quick start and core concepts
├── workspaces/         # Workspace management
├── repositories/       # File organization
├── parts/              # Genetic parts library
├── constructs/         # Construct design
├── sequence-tools/     # Sequence viewer and analysis
├── compiler-simulation/# Compiler and simulation
├── inventory/          # Physical sample tracking
├── tools/              # BLAST, SecureDNA, export
├── kernel-ai/          # AI assistant
├── settings/           # Account configuration
├── developer/          # API documentation
├── resources/          # FAQ and support
└── screenshots/        # Documentation images
```

## Publishing

This repository is connected to GitBook. Changes pushed to the `product-docs-from-template` branch are automatically published to https://docs.kernel.asimov.com.

## Contributing

For internal contributors: edit markdown files in `product-docs/` and update `SUMMARY.md` for navigation changes.
