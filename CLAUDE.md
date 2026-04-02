# CLAUDE.md — Super Core Solutions LLC Website

## Project Overview

Marketing website for Super Core Solutions LLC. Dual-purpose: sells enterprise identity/automation consulting and AI-accelerated application development services. Hosted on GitHub Pages at supercoresolutionsllc.com.

- **Repo**: `supercoresolutionsllc-site`
- **Deployment**: Auto-deploys on push to `main` via GitHub Pages
- **Domain**: supercoresolutionsllc.com (configured via CNAME file)
- **No build step** — plain HTML/CSS/JS, no bundler or framework

## Site Structure

| File | Purpose |
|------|---------|
| `index.html` | Homepage (hero, services overview, featured work, credibility strip, CTA) |
| `contact.html` | Contact info (email, phone, location) |
| `portfolio.html` | Case studies (TrainBJJ, BrewRoute, additional work) |
| `about.html` | Professional background, approach, certifications |
| `services/identity-automation.html` | Identity & Automation service detail page |
| `services/app-development.html` | Application Development service detail page |
| `privacy.html` | Privacy policy (Train BJJ) |
| `terms.html` | Terms of service (Train BJJ) |
| `support.html` | Support page with FAQ |
| `styles.css` | Complete design system (single file) |
| `script.js` | Hamburger menu, services dropdown, scroll fade-in animations |
| `CNAME` | GitHub Pages custom domain config |
| `.nojekyll` | Disables Jekyll processing |

## Design System

### Color Palette (CSS Variables)

| Variable | Value | Usage |
|----------|-------|-------|
| `--color-primary` | `#2B5C8A` | Steel blue — links, icons, borders |
| `--color-primary-light` | `#3A7AB8` | Hover states |
| `--color-accent` | `#E8853D` | Warm amber — CTAs, highlights |
| `--color-accent-hover` | `#D4732E` | Accent hover |
| `--color-dark` | `#0F172A` | Footer, dark sections |
| `--color-bg` | `#F8FAFC` | Page backgrounds |
| `--color-bg-alt` | `#F1F5F9` | Alternating sections |
| `--color-card` | `#FFFFFF` | Card backgrounds |
| `--color-text` | `#1E293B` | Primary text |
| `--color-text-secondary` | `#64748B` | Secondary text |
| `--color-border` | `#E2E8F0` | Borders |

### Typography
- **Font**: Inter (Google Fonts) with system font fallback
- **Headings**: 700-800 weight, negative letter-spacing
- **Body**: 400-500 weight, 1.6 line-height

### Layout
- Max content width: 1200px
- Card border-radius: 12px
- Responsive breakpoints: 768px (tablet), 480px (mobile)
- Scroll fade-in animations via IntersectionObserver

### Component Patterns
- **Service cards**: Icon + title + description + "Learn more" arrow link
- **Portfolio cards**: Status badge + title + description + tech pills + link
- **Tech pills**: Small rounded badges (`tech-pill` class)
- **Credibility strip**: Horizontal icons + text items
- **CTA sections**: Full-width primary background + headline + button
- **Offering cards**: Numbered items with descriptions

## Navigation

- **Desktop**: Sticky nav with Services dropdown, Portfolio, About, Contact (accent CTA button)
- **Mobile**: Hamburger menu → full-width slide-down panel with collapsible Services submenu
- **Services dropdown**: Click-to-toggle (not hover), closes on outside click

## Content Rules

- **Do NOT mention**: UKG Sync, SSPR Portal, specific current employer name in case studies
- **No pricing** — all engagements are custom-scoped
- **Contact**: superd@supercoresolutionsllc.com, (330) 984-9249, Pennsylvania

## Contact Info

- Business email: superd@supercoresolutionsllc.com
- Phone: (330) 984-9249
- Product support: Support@trainbjjapp.com
- AI feedback: AIFeedback@trainbjjapp.com
