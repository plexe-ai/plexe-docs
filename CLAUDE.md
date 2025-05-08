# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains documentation for Plexe.ai, a machine learning model generation platform, built with Mintlify (a documentation site generator). The documentation describes Plexe's capabilities, API reference, and use cases.

## Development Commands

### Local Development

To run the documentation site locally:

```bash
# Install Mintlify CLI globally
npm install -g mint

# Start the development server
mint dev
```

This will start a local development server, typically on port 3000.

### Building and Deploying

Mintlify handles deployment automatically when changes are pushed to the main branch. No additional build commands are needed.

## Documentation Structure

- `mint.json`: Configuration file for the Mintlify documentation site, including navigation structure, colors, and metadata.
- `introduction/`: Contains introductory documents about Plexe
- `api-reference/`: API documentation including endpoints and usage instructions
- `essentials/`: Core documentation including explanations, guides, and references
- `usecases/`: Example use cases organized by industry/application

## Content Format

Documentation content is written in MDX (Markdown with JSX support). Each content file follows this structure:

```mdx
---
title: "Page Title"
---

Content in Markdown format...
```

## Documentation Updating Guidelines

1. Edit existing MDX files to update content, or add new files for new sections.
2. Update `mint.json` to include any new files in the navigation structure.
3. Follow existing formatting patterns for consistency.
4. Use headings (###) appropriately for document structure.
5. Include code examples where relevant for API usage.