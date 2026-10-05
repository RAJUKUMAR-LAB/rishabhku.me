# OSCA India Digital Marketing Agency Website

## Overview
This project is a premium, conversion-focused marketing website for OSCA India Digital Marketing Agency. It is built as a static Single Page Application with dynamic client-side routing, service detail pages, lead capture workflows, and trust-focused sections (including Google Business profile and reviews).

The website is designed to help visitors move quickly from discovery to inquiry through strong call-to-actions, WhatsApp-first communication, and structured service presentation.

## Live Website
Production URL:
https://oscaindia.vercel.app

## Project Type
- Static frontend website
- Single Page Application (SPA)
- Path-based routing with fallback rewrite
- No backend app server required for normal page rendering

## Tech Stack
- HTML5
- CSS3 (custom design system)
- Vanilla JavaScript (no frontend framework)
- Vercel hosting and deployment

## Core Files
- index.html: app shell
- assets/css/style.css: full UI system, components, and responsive breakpoints
- assets/js/app.js: routing, rendering, data models, forms, integrations, and interactivity
- vercel.json: SPA rewrite config for clean URL access

## Key Functional Areas

### 1) Routing and Page Rendering
The website uses client-side route resolution and dynamic rendering. It supports clean URLs and also normalizes older hash-style links.

Main page routes include:
- Home
- About
- Team
- Services
- Service detail pages (dynamic)
- Start Project
- Contact
- Landing
- Privacy Policy
- Terms

Behavior highlights:
- Canonical path mapping for cleaner URLs
- History API navigation
- Popstate handling for browser back/forward
- Dynamic metadata update per page

### 2) Service System
The platform uses centralized service data objects to keep pages and forms consistent.

Current major services:
- Website Development
- E-commerce Development
- SEO Optimization
- Ads
- Social Media Marketing
- Political Social Media Management
- YouTube Monetization
- Facebook Management
- Branding and Design
- App Development
- Content Marketing
- Marketing Automation

Each service includes:
- Short positioning line
- Benefits
- Features
- Process steps
- Pricing range
- Mini-service types
- FAQ entries
- Start Project pricing context

### 3) Lead Capture and Contact Flow
Lead generation is the primary business objective. Forms appear across key pages and are processed through a unified submit handler.

Lead data captured includes:
- Name
- Phone
- Email
- Company
- Selected service and optional mini-service
- Budget and timeline
- Requirement message
- Contact preference (WhatsApp or Email)
- Source context

Delivery flow:
- WhatsApp mode builds a detailed prefilled message
- Email mode builds a structured inquiry email body
- Leads are stored in local storage
- Optional CRM webhook and auto-email endpoint calls are supported

### 4) WhatsApp-first CTA System
The site has a strong WhatsApp-first communication model.

Features:
- Multi-number WhatsApp dropdown options
- Floating WhatsApp quick-action button
- Context-aware WhatsApp lead message composition
- Auto-hide dropdown behavior for cleaner interaction

### 5) Google Business Trust Layer
Google credibility is integrated across the site through dedicated sections.

Included elements:
- Google Business profile link
- Embedded location map
- Review highlight cards
- Auto-running review marquee
- Additional review-focused trust cards in universal sections

### 6) Universal Footer-Adjacent Growth Sections
Most non-landing pages append a common trust and conversion stack above the footer.

Includes:
- Performance impact snapshot
- Why choose OSCA section
- Google review highlights
- Google business presence section
- Next-step CTA block

### 7) UI and Visual Direction
Design language focuses on premium light glassmorphism with conversion-first hierarchy.

Highlights:
- Layered card and surface system
- Brand-driven gradients and atmospheric background depth
- Strong CTA treatment
- Premium typography
- Consistent section spacing and visual rhythm

## Responsive Behavior
The website includes comprehensive responsive handling for desktop, tablet, and mobile.

Notable adaptations:
- Responsive navigation with toggle menu
- Compact CTA and floating action behavior on small screens
- Service grids and section stacks adapt by breakpoint
- Review marquee and card layouts adapt for small devices
- Ultra-small screen navigation compaction added for better header fit

## SEO and Metadata
Dynamic page-level metadata is handled in JavaScript.

Includes:
- Route-based title and description updates
- Structured schema updates for better search context
- Canonical path consistency through route normalization

## Analytics and Event Tracking
Tracking hooks are included for user action observability.

Tracked interactions:
- Page view events
- CTA click events
- Lead form submission events

Tracking scripts are initialized in deferred/non-blocking style for better initial UX.

## Deployment
Deployment is done on Vercel production.

Important setup:
- vercel.json rewrites all paths to index.html
- This ensures direct URL access works for SPA routes

Typical deploy command:
- npx vercel --prod --yes

## Current Production Health
Recent checks confirm production route responds successfully:
- https://oscaindia.vercel.app returns HTTP 200

## Known Integration Placeholders
Some integration constants are intentionally placeholders and should be replaced with real values if needed:
- GA measurement ID
- Meta Pixel ID
- CRM webhook endpoint
- Auto-email endpoint

## Suggested Handover Notes
If sharing this project with another developer or agency, provide:
- Vercel project access
- Domain/alias control access
- Google Business profile ownership/editor access
- WhatsApp business number ownership
- Final approved pricing/service updates policy
- Lead handling workflow owner (sales/contact person)

## Maintenance Checklist
- Validate all routes after every deployment
- Recheck mobile navigation and floating CTA overlap on small screens
- Keep service data and pricing synchronized across all maps
- Verify WhatsApp message fields after form changes
- Periodically refresh Google review dataset from approved source
- Keep contact emails and phone numbers up to date

## License / Usage
This codebase is business website implementation for OSCA India Digital Marketing Agency operations. Use and redistribution should follow owner permission and branding rights.
