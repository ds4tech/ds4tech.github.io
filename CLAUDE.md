# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based GitHub Pages website for ds4tech's consulting services. The site uses the midnight theme and showcases DevOps, SRE, and infrastructure consulting expertise.

## Development Commands

### Local Development
```bash
bundle install          # Install Ruby dependencies
bundle exec jekyll serve # Start local development server
```

### Site Building
```bash
bundle exec jekyll build # Build the site for production
```

## Architecture and Structure

### Jekyll Configuration
- Uses Jekyll 4.3.x with the midnight remote theme (`pages-themes/midnight@v0.2.0`)
- Site configuration in `_config.yml` defines metadata, theme, and plugins
- Markdown processing via kramdown

### Content Structure
- `index.markdown`: Main landing page with consulting services content
- `_posts/`: Blog posts directory (standard Jekyll convention)
- `_layouts/default.html`: Custom layout template overriding theme defaults
- `assets/css/style.scss`: Custom styling (SCSS preprocessing)
- `about.markdown`: About page
- `404.html`: Custom error page

### Theme and Styling
- Base theme: GitHub Pages midnight theme
- Custom styles can be added via `assets/css/style.scss`
- Layout customization through `_layouts/` directory

### Content Management
- Front matter in markdown files controls page metadata and layout
- Site variables (title, email, etc.) defined in `_config.yml` and accessible via `{{ site.variable }}`
- Content uses Jekyll's Liquid templating system

### Deployment
- Automatically deployed to GitHub Pages when changes are pushed to main branch
- No manual build/deployment process required for GitHub Pages hosting