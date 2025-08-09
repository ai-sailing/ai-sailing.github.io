# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
- **Type**: Hugo static site generator with PaperMod theme
- **Purpose**: "Sailing with AI" blog/documentation site
- **Deployment**: GitHub Pages (`ai-sailing.github.io`)

## Key Commands

### Development
- `hugo server` - Start development server with live reload
- `hugo server --buildDrafts` - Include draft content
- `hugo` - Build site to `/docs` directory
- `hugo --buildDrafts --gc` - Build with drafts and garbage collection

### Content Management
- Content goes in `/content/` directory
- Posts: `/content/posts/`
- Pages: `/content/` (e.g., `/content/about.md`)
- Static files: `/static/` directory

### Configuration
- Main config: `hugo.toml`
- Theme config: `/themes/PaperMod/` (don't modify directly)
- Custom layouts: `/layouts/` (override theme defaults)
- Custom assets: `/assets/` (CSS, JS)

## Architecture Notes
- **Build output**: `/docs/` (used by GitHub Pages)
- **Theme**: PaperMod submodule - use custom layouts to override
- **Internationalization**: `/i18n/` directory configured
- **Archetypes**: `/archetypes/` for content templates

## Requirements
- Hugo 0.146.0+ required
- GitHub Actions workflow included for deployment
- No Node.js dependencies (empty package.json)