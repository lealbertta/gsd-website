# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the marketing website for **GSD (Get Stuff Done)**, a SwiftUI iOS application focused on daily goal/task management. The website serves as the primary marketing presence to promote the app and drive downloads.

**Live Website**: https://lealbertta.github.io/gsd-website

## Technology Stack

- **Astro 5**: Modern static site generator for optimal performance
- **Tailwind CSS**: Utility-first CSS framework for rapid styling  
- **TypeScript**: Type-safe development
- **GitHub Pages**: Automated deployment

## Commands

### Development
```bash
npm install          # Install dependencies
npm run dev         # Start development server (localhost:4321)
npm run build       # Build for production
npm run preview     # Preview production build
```

### Code Quality
```bash
npm run lint        # Run ESLint
npm run lint:fix    # Auto-fix ESLint issues
npm run format      # Format code with Prettier
npm run format:check # Check formatting
npm run check       # Run all checks (format + lint)
```

## Architecture

### Core Framework
- **Astro**: Zero JavaScript by default, island architecture for optimal performance
- **Tailwind**: Utility-first styling with modern CSS features
- **Static Generation**: All pages pre-rendered for fast loading

### File Structure
```
src/
├── pages/
│   └── index.astro         # Main landing page
├── styles/
│   └── global.css          # Tailwind imports and global styles
└── components/             # Reusable Astro components (future)

public/
├── favicon.svg             # Site favicon
└── images/                 # App screenshots, marketing assets
```

### Deployment Configuration
- **Base URL**: `/gsd-website` (configured in astro.config.mjs)
- **Site URL**: `https://lealbertta.github.io`
- **GitHub Actions**: Automated deployment on push to main

## Content Strategy

The website follows a focused marketing approach with key sections:
- **Hero**: "One Goal. Every Day." value proposition
- **Features**: Three core benefits (One Goal Focus, Sliding Completion, Daily Themes)
- **How It Works**: Simple 3-step process
- **Download**: App Store integration with iOS requirements

## iOS App Context

For detailed information about the GSD iOS app, its features, design philosophy, and how it relates to this marketing website, see:

**[claude/gsd-ios-app-context.md](claude/gsd-ios-app-context.md)**

This context file provides comprehensive background on:
- GSD app's core concept and features
- Target audience and messaging strategy
- Design guidelines and brand consistency
- Content updates and marketing considerations