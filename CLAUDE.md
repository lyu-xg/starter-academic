# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Academic personal website for Xueguang Lyu built with Hugo static site generator and Wowchemy theme. Deployed to https://xue-guang.com via Netlify.

## Common Commands

```bash
# Start development server
bash view.sh
# or directly:
hugo server --disableFastRender --i18n-warnings

# Production build
hugo --gc --minify -b https://xue-guang.com

# Update Wowchemy theme modules
bash update_wowchemy.sh
```

## Architecture

**Configuration**: Split across `config/_default/` directory
- `config.toml` - Hugo core settings, module imports, permalinks
- `params.toml` - Theme settings, features (math, diagrams), analytics, contact info
- `menus.toml` - Navigation menu items
- `languages.toml` - Language configuration (English only)

**Content Structure**: All in `content/` using Markdown with YAML frontmatter
- `home/` - Widget-based homepage sections (each .md file is a widget, `headless: true`)
- `post/` - Blog posts (each post in its own directory with index.md)
- `publication/` - Research papers (each in own directory, follows academic citation format)
- `authors/admin/` - Primary author profile with avatar

**Static Assets**: `static/` directory
- `media/` - PDFs (CV, research statement)
- `admin/` - Netlify CMS configuration

**Theme Customization**:
- `data/fonts/` - Custom font definitions
- `data/themes/` - Theme overrides
- `layouts/partials/` - Template overrides

## Key Patterns

- Homepage uses Wowchemy's widget system where frontmatter controls display order (`weight`), activation (`active`), and layout
- Publications use MLA citation style with structured frontmatter for authors, dates, DOIs
- Go modules manage theme dependencies (see `go.mod`)
- Netlify handles CI/CD with context-specific builds defined in `netlify.toml`
