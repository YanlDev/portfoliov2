# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio website built with Astro, Tailwind CSS, and TypeScript. It showcases Milder Carreón's professional background as a Full Stack Developer and Industrial Engineer.

## Essential Commands

- `npm install` - Install dependencies
- `npm run dev` - Start development server at localhost:4321
- `npm run build` - Build production site to ./dist/
- `npm run preview` - Preview production build locally

## Architecture

### Framework & Stack
- **Astro**: Static site generator with component-based architecture
- **Tailwind CSS v4**: Utility-first CSS framework with @theme configuration
- **TypeScript**: Type safety with strict configuration
- **Font Awesome**: Icon library loaded via CDN

### Key Components
- `src/layouts/Layout.astro` - Base HTML layout with meta tags and Font Awesome integration
- `src/components/Portafolio.astro` - Main portfolio component containing all page sections
- `src/pages/index.astro` - Entry point that combines Layout and Portafolio components

### Styling Architecture
- Global styles in `src/styles/global.css` with Inter font and Tailwind imports
- Component-specific styles using Astro's scoped `<style>` tags
- Tailwind configuration through `@theme` directive in CSS

### Interactive Features
- Scroll-snap navigation between sections
- Intersection Observer for active navigation states
- Smooth scrolling behavior
- Responsive design with sidebar and main content areas

## File Structure
```
src/
├── components/          # Reusable Astro components
├── layouts/            # Base layouts
├── pages/              # Route-based pages
├── styles/             # Global CSS and Tailwind config
└── icons/              # Static technology logos
```

## Development Notes

- The portfolio uses a two-column layout: fixed sidebar (navigation) and scrollable main content
- Navigation links use data attributes for section targeting
- Tech stack logos are imported as static assets and displayed with hover effects
- CSS uses modern features like scroll-snap and Intersection Observer API