# Plexe Documentation

This repository contains the documentation for Plexe, which consists of:

1. The open-source Python library (`pip install plexe`)
2. The proprietary Plexe Platform (`console.plexe.ai`/`api.plexe.ai`)

The documentation is built using [Mintlify](https://mintlify.com), a modern documentation platform.

## Local Development

```bash
# Install Mintlify CLI globally
npm install -g mint

# Start the documentation site locally
mint dev
```

This will start a local development server, typically on port 3000.

## Documentation Structure

- `mint.json`: Configuration file with navigation structure, colors, and metadata
- `introduction/`: Introductory content about Plexe
- `library/`: Documentation for the open-source Python library
  - `tutorials/`: Step-by-step guides
  - `how-to/`: Task-oriented guides
  - `explanation/`: Concept explanations
  - `reference/`: API reference
- `platform/`: Documentation for the Plexe Platform
  - Similar structure to the library section
- `api-reference/`: API documentation including endpoints

## Content Format

Content is written in MDX (Markdown with JSX support). Files follow this structure:

```mdx
---
title: "Page Title"
description: "Brief description of the page"
---

Content in Markdown format with optional JSX components...
```

## Deployment

Mintlify handles deployment automatically when changes are pushed to the main branch. No additional build commands are required.

## Contributing

1. Create a new branch for your changes
2. Edit existing MDX files or add new ones
3. Update `mint.json` if adding new pages to the navigation
4. Test locally with `mint dev`
5. Submit a pull request to the main branch