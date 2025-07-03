# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Cortex Vision is a static medical technology company website presenting three neurosurgical planning software products (ABIGAIL, BRAIN, and BRIDGE). The site is built with pure HTML/CSS and deployed via GitHub Pages.

## Commands

### Development
- **View site locally**: Open `index.html` directly in a web browser
- **Deploy**: Push to `main` branch - GitHub Actions automatically deploys to https://cortexvision.eu

### Common Tasks
- **Update content**: Edit `index.html` directly
- **Add images**: Place in `assets/imgs/` directory
- **Modify styles**: Update the inline CSS in `index.html`

## Architecture

This is a single-page static website with:
- **index.html**: Contains all content, structure, and inline styles
- **assets/imgs/**: Static image resources (logo.png, logo.jpg, background.jpg)
- **GitHub Actions**: Automated deployment pipeline to GitHub Pages on main branch push

## Key Design Patterns

1. **Styling**: All CSS is inline within `index.html` using:
   - Purple accent color: `#88314f`
   - Semi-transparent overlays for readability
   - Responsive grid layout for team members
   - Fixed background with gradient overlay

2. **Content Structure**:
   - Products section with detailed software descriptions
   - Team section with member profiles in grid layout
   - Publications section with academic references

3. **No Build Process**: Direct HTML/CSS editing with immediate results

## Important Notes

- **Custom Domain**: Configured via CNAME file for cortexvision.eu
- **Deployment**: Automatic via GitHub Actions - no manual deployment needed
- **Images**: Keep file sizes reasonable for web performance
- **Browser Compatibility**: Uses modern CSS features (grid, flexbox) - test in modern browsers