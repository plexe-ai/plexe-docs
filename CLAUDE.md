# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains documentation for Plexe.ai, a machine learning model generation platform, built 
with Mintlify (a documentation site generator). The documentation describes Plexe's capabilities, API reference, 
and use cases.

The Plexe platform consists of:
1. An open-source Python library (`pip install plexe`)
2. The proprietary Plexe Platform (`console.plexe.ai`/`api.plexe.ai`)

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

- `docs.json`: Configuration file for the Mintlify documentation site, including navigation structure, colors, and metadata.
- `pages/`: Contains all documentation content
  - `introduction/`: Introductory content about Plexe
  - `library/`: Documentation for the open-source Python library
    - `tutorials/`: Step-by-step guides
    - `how-to/`: Task-oriented guides
    - `explanation/`: Concept explanations
    - `reference/`: API reference
  - `platform/`: Documentation for the Plexe Platform
    - Similar structure to the library section
  - `usecases/`: Example use cases showing how Plexe can be applied

## Content Format

Documentation content is written in MDX (Markdown with JSX support). Each content file follows this structure:

```mdx
---
title: "Page Title"
description: "Brief description of the page"
---

Content in Markdown format with optional JSX components...
```

## Documentation Workflow

1. Create a new branch for your changes
2. Edit existing MDX files or add new ones
3. Update `docs.json` if adding new pages to the navigation
4. Test locally with `mint dev`
5. Submit a pull request to the main branch

## Helper Scripts

- `scripts/dumpdocs.py`: Collects all documentation files and outputs them to a single text file, useful for providing 
  context to large language models.