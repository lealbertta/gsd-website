# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with the GSD marketing website.

## Project Overview

This is the marketing website for **GSD (Get Stuff Done)**, a SwiftUI iOS application focused on daily goal/task management. The website serves as the primary marketing presence to promote the app and drive downloads.

**Main iOS App Repository**: https://github.com/lealbertta/GSD  
**Project Board**: https://github.com/users/lealbertta/projects/2/views/1  
**Live Website**: https://lealbertta.github.io/gsd-website

## About GSD iOS App

### Core Concept
GSD is built around **radical simplicity**: users can set only **one goal per day**. This constraint eliminates decision fatigue and endless todo lists, helping users focus on what truly matters.

### Key App Features
- **One Goal Focus**: Set one meaningful goal per day, no overwhelming lists
- **Sliding Completion**: Complete goals with a satisfying slide gesture
- **Daily Themes**: Each day has unique color themes (Monday = Blue, Tuesday = Red, etc.)
- **Today/Tomorrow Interface**: Simple tab system for planning ahead
- **Personalized Greetings**: Day-specific welcome messages and completion celebrations

### App Architecture (for context)
- **Framework**: SwiftUI with The Composable Architecture (TCA)
- **Data**: SwiftData for persistence
- **Design**: Inter font family, extensive color palette (100-900 scale)
- **UX**: Sliding card interface, one-handed operation focus

## Website Technology Stack

### Core Framework
- **Astro 5**: Modern static site generator for optimal performance
- **Tailwind CSS**: Utility-first CSS framework for rapid styling
- **TypeScript**: Type-safe development

### Development Tooling
- **ESLint**: Code linting with TypeScript and Astro support
- **Prettier**: Code formatting with Astro plugin
- **GitHub Actions**: Automated deployment to GitHub Pages

### Performance Features
- **Zero JavaScript by default**: Astro's island architecture
- **Optimized builds**: Automatic asset optimization and compression
- **Fast loading**: Minimal bundle size for quick page loads

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

## Website Content Strategy

### Target Audience
- **Primary**: Productivity-focused individuals overwhelmed by complex task management
- **Secondary**: iOS users seeking simple, elegant daily planning tools
- **Demographic**: Tech-savvy professionals, students, anyone struggling with todo list fatigue

### Key Messaging
1. **"One Goal. Every Day."** - Core value proposition
2. **Simplicity over complexity** - Anti-feature philosophy
3. **Focus over overwhelm** - Solution to decision fatigue
4. **Daily consistency** - Building better habits through constraints

### Content Sections
- **Hero**: Compelling value proposition with clear CTA
- **Features**: Three core benefits (One Goal Focus, Sliding Completion, Daily Themes)
- **How It Works**: Simple 3-step process
- **Download**: App Store integration with iOS requirements
- **Social Proof**: Testimonials and usage statistics (when available)

## File Structure

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

.github/workflows/
└── deploy.yml              # GitHub Pages deployment
```

## Design Guidelines

### Visual Identity
- **Colors**: Reflect app's day-specific themes (blues, reds, purples, etc.)
- **Typography**: Clean, readable sans-serif (system fonts)
- **Layout**: Minimal, focused design matching app's simplicity philosophy
- **Images**: App screenshots, mockups showing the sliding interface

### Responsive Design
- **Mobile-first**: Primary target is iOS users
- **Tablet/Desktop**: Enhanced experience with larger content areas
- **Touch-friendly**: Large CTAs and interactive elements

### Performance Targets
- **Core Web Vitals**: Excellent scores across all metrics
- **Load Time**: Sub-1 second initial page load
- **Bundle Size**: Minimal JavaScript, optimized assets

## Deployment

### Hosting
- **Platform**: GitHub Pages (free, reliable)
- **URL**: https://lealbertta.github.io/gsd-website
- **SSL**: Automatic HTTPS via GitHub Pages

### Deployment Process
1. Push to `main` branch triggers GitHub Action
2. Astro build process generates static site
3. Deployment to GitHub Pages environment
4. Live site updated automatically

### Environment Configuration
- **Base URL**: `/gsd-website` (configured in astro.config.mjs)
- **Site URL**: `https://lealbertta.github.io`
- **Build Output**: `dist/` directory (ignored in git)

## Content Updates

### Regular Updates
- **App Store link**: Update when app is published
- **Screenshots**: Refresh with latest app UI
- **Testimonials**: Add user feedback and reviews
- **Feature highlights**: Update based on app development

### Marketing Campaigns
- **Launch announcement**: Major updates to hero section
- **Feature releases**: New sections for significant app updates
- **Press coverage**: Add media mentions and reviews

## SEO Strategy

### Meta Information
- **Title**: "GSD - Get Stuff Done | Daily Goal Tracking Made Simple"
- **Description**: Focus on key benefits and target keywords
- **Keywords**: "daily goals", "productivity app", "simple task management", "iOS planning"

### Content Optimization
- **Headings**: Clear hierarchy with target keywords
- **Alt text**: Descriptive image captions for accessibility
- **Schema markup**: App/software markup for rich snippets (future)

## Analytics & Monitoring

### Metrics to Track
- **Page views**: Overall site traffic
- **Bounce rate**: Content engagement quality
- **App Store clicks**: Conversion tracking
- **Device breakdown**: iOS vs other platforms

### Performance Monitoring
- **Core Web Vitals**: Lighthouse CI integration
- **Load times**: Real user monitoring
- **Error tracking**: Build and runtime error monitoring

## Important Considerations

### Brand Consistency
- Maintain alignment with iOS app's visual identity
- Use same terminology and messaging as in-app copy
- Reflect the app's core philosophy of simplicity

### User Journey
- **Discovery**: SEO, social media, word of mouth
- **Evaluation**: Website explains value proposition clearly
- **Conversion**: Smooth path to App Store download
- **Retention**: Set expectations for app experience

### Future Enhancements
- **Blog section**: Productivity tips, user stories
- **Testimonials**: Customer success stories
- **Integration demos**: Video walkthroughs of key features
- **Pricing**: If app moves to premium model

Remember: This website should embody the same simplicity and focus that makes the GSD app special. Every element should serve the goal of converting visitors into app users while accurately representing the product's core value proposition.