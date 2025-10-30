# BamTech Website AI Development Guide

This guide provides essential context for AI agents working with the BamTech website codebase.

## Project Overview
- Single-page marketing website for BamTech Limited, focusing on cybersecurity and IT consulting services
- Built with HTML, TailwindCSS, and vanilla JavaScript
- Uses CDN-hosted dependencies for simplicity

## Key Technologies
- TailwindCSS (via CDN): `https://cdn.tailwindcss.com`
- Lucide Icons (via CDN): `https://unpkg.com/lucide@latest/dist/umd/lucide.js`
- Google Fonts: Inter font family

## Project Structure
```
index.html          # Single-page application
.github/            # GitHub-specific configurations
```

## Design System
### Colors
The project uses a custom color system defined in CSS variables:
```css
--primary-color: #00A8E8    /* Vibrant Blue - main accent */
--secondary-color: #0047AB  /* Deep Blue - alternative accent */
--background-dark: #1F2937  /* Gray 800 - section backgrounds */
--background-darker: #111827/* Gray 900 - main background */
--text-light: #E5E7EB      /* Light Gray - text */
```

### Custom Classes
- `.text-primary`: Primary blue text color
- `.bg-primary`: Primary blue background
- `.border-primary`: Primary blue border
- `.hover:bg-primary-dark`: Darker blue on hover (#0099D4)

## Component Patterns
1. **Section Headers**: Use scroll-margin-top for proper anchor navigation
2. **Logo Circle**: Standardized 44px container with 32px image
3. **Hero Section**: Includes slider with dark overlay for text readability
4. **Mobile Menu**: Toggle animation between open/close states

## Development Workflow
1. Preview changes using a local server (e.g., Live Server VS Code extension)
2. Test responsive layouts across different viewport sizes
3. Validate changes in modern browsers (Chrome, Firefox, Safari)

## Best Practices
- Maintain consistent use of CSS variables for theming
- Follow TailwindCSS class ordering conventions
- Ensure responsive design works at all breakpoints
- Keep accessibility in mind with proper ARIA attributes and semantic HTML

When making changes:
1. Preserve the existing color scheme and design system
2. Maintain mobile-first responsive approach
3. Follow established component patterns
4. Test interactive elements across devices