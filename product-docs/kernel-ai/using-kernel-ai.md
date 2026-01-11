# Using Kernel AI

Get AI assistance for genetic design tasks and navigation.

## What is Kernel AI?

Kernel AI is an AI assistant that helps you:
- Navigate the Kernel interface
- Answer genetic design questions
- Find constructs and parts
- Explain biological concepts
- Assist with design decisions

## Accessing Kernel AI

### Sidebar

Click **Kernel AI** in the left sidebar to open the chat interface.

![Kernel AI Interface](../screenshots/kernel-ai.png)

### In-Editor

Click **AI** in the construct editor's right sidebar for context-aware assistance.

### Keyboard Shortcut

Press **Cmd/Ctrl + K** to quickly access Kernel AI.

## What You Can Ask

### Navigation

Ask Kernel AI to help you find things:
- "Take me to my recent constructs"
- "Find all promoters in my workspace"
- "Show me the CMV constructs"
- "Open the shared parts repository"

### Design Questions

Get help with genetic design:
- "What promoter should I use for high expression in CHO cells?"
- "Explain the difference between SV40 and BGH terminators"
- "How do I optimize this sequence for E. coli?"
- "What signal peptide works best for secretion?"

### Construct Information

Ask about your designs:
- "What parts are in this construct?"
- "Show me the sequence of the heavy chain"
- "What's the GC content of this region?"
- "Are there any HindIII sites?"

### Workflow Help

Get guidance on tasks:
- "How do I create a new construct?"
- "How do I share a repository?"
- "How do I run a simulation?"
- "How do I export as GenBank?"

## Example Conversations

### Finding Parts

**You**: Find all T7 promoters in my workspace

**Kernel AI**: I found 3 T7 promoter parts in your workspace:
1. T7-Promoter (in Team Parts)
2. T7-Strong-Promoter (in Expression Library)
3. T7-Lac-Promoter (in Inducible Parts)

Would you like me to open any of these?

### Design Advice

**You**: What's the best way to express an antibody in HEK293?

**Kernel AI**: For antibody expression in HEK293 cells, I recommend:
- CMV or EF1α promoter for strong expression
- IgK or native signal peptide for secretion
- BGH poly(A) for 3' UTR
- Consider dual-plasmid system for HC + LC

Would you like me to help you set up a construct with these elements?

### Navigation

**You**: Take me to the construct I was working on yesterday

**Kernel AI**: Based on your recent activity, you were working on:
- HC-Expression-v3 (modified 18 hours ago)
- LC-Optimized (modified 20 hours ago)

Which one would you like to open?

## Tips for Effective Use

### Be Specific

More specific questions get better answers:
- Instead of "help with my construct"
- Try "help me add a His-tag to the C-terminus of my protein"

### Provide Context

Include relevant details:
- The construct you're working on
- Your expression system
- What you're trying to achieve

### Ask Follow-ups

Continue the conversation:
- Ask for more details
- Request alternatives
- Get step-by-step guidance

## Capabilities

### What Kernel AI Can Do

- Search and navigate workspace content
- Explain genetic concepts
- Recommend parts and designs
- Guide you through workflows
- Answer questions about Kernel features

### Limitations

- Cannot modify constructs directly (you make the changes)
- Answers based on general knowledge and your workspace
- Complex designs may need expert review
- Experimental predictions should be validated

## Best Practices

### Design Assistance

- Use AI for initial guidance
- Verify recommendations
- Consider multiple approaches
- Validate critical designs

### Learning

- Ask "why" questions to learn
- Request explanations of concepts
- Explore alternatives

## Next Steps

- [Quick Start Guide](../getting-started/quick-start.md) — Get started with Kernel
- [Creating Constructs](../constructs/creating-constructs.md) — Design with AI help
- [Part Library](../parts/part-library.md) — Find parts AI recommends
