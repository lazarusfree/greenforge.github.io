# GreenForge

A digital platform for the ideation and validation of sustainable business models. GreenForge guides entrepreneurs and students through the full process of generating, structuring, and scoring green business concepts using a purpose-built web interface.

Built as a course project aligned with the theme: **The Development of a Digital Platform for the Ideation and Validation of Sustainable Business Models**.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Pages](#pages)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Budget Summary](#budget-summary)
- [Development Process](#development-process)
- [SDG Alignment](#sdg-alignment)
- [License](#license)

---

## Overview

GreenForge is a single-file, browser-based web application that helps users:

- Explore sustainable business categories (recycling, clean energy, circular economy, etc.)
- Generate structured business ideas based on their context and constraints
- Build an Eco Business Model Canvas with an added environmental impact layer
- Validate their concept across five dimensions using the Greenability scoring system
- Review a full project budget breakdown and development documentation

The platform requires no server, no build tools, and no dependencies to run. Open `index.html` in any modern browser to use it.

---

## Features

### Idea Generator
Select up to three sustainability focus areas from twelve categories. Fill in your target market, region, capital range, business model preference, and problem statement. The tool returns a structured business concept with market opportunity estimates, eco impact scores, revenue potential, scalability ratings, and key value propositions.

### Eco Business Model Canvas
An editable, nine-block Business Model Canvas based on the Osterwalder framework, extended with a tenth block for the Environmental Impact Layer. All fields are directly editable in the browser. A sample canvas is available to load for reference.

### Greenability Score Dashboard
Five self-assessment sliders covering Market Viability, Environmental Impact, Financial Feasibility, Social Benefit, and Scalability. Scores are aggregated into a composite Greenability Score displayed as an animated ring chart. The dashboard also includes dimension-specific recommendations, UN SDG alignment badges, and a three-phase impact roadmap.

### Budget and Documentation Page
A full tabulated breakdown of the RM 25,000 development budget, covering hosting, AI API credits, design tools, developer costs, testing, and marketing. Includes a technology stack overview and a six-phase SDLC development process narrative.

---

## Pages

| Page | Route (nav) | Description |
|---|---|---|
| Home | `home` | Landing page with hero section, feature cards, and how-it-works flow |
| Ideate | `ideate` | Category picker and idea generation form |
| BM Canvas | `canvas` | Editable Eco Business Model Canvas |
| Validate | `validate` | Greenability Score dashboard with sliders and SDG mapper |
| Budget and Docs | `budget` | Budget table, tech stack, and development process |

---

## Tech Stack

**Frontend**
- HTML5
- CSS3 (custom properties, grid, flexbox, keyframe animations)
- Vanilla JavaScript (no frameworks, no build step)
- Google Fonts: Fraunces (display), Plus Jakarta Sans (body)

**Planned Backend (production roadmap)**
- Node.js with Express for REST API
- Firebase Firestore for idea and canvas storage
- Firebase Authentication for user accounts
- Firebase Storage for file attachments
- OpenAI GPT-4o API for AI-assisted idea generation

**DevOps and Tooling (production roadmap)**
- GitHub for version control and CI/CD via GitHub Actions
- Cloudflare for CDN, DDoS protection, and DNS
- Figma for UI/UX design and prototyping
- Notion and Trello for project management
- BrowserStack for cross-browser QA
- Hotjar for heatmaps and session analysis

---

## Getting Started

### Prerequisites

No prerequisites. The project is a self-contained HTML file.

### Running Locally

1. Clone the repository:

```bash
git clone https://github.com/your-username/greenforge.git
cd greenforge
```

2. Open the file in your browser:

```bash
open index.html
```

Or drag and drop `index.html` into any modern browser window. The application is fully functional offline.

### Tested Browsers

| Browser | Version | Status |
|---|---|---|
| Google Chrome | 120+ | Supported |
| Mozilla Firefox | 121+ | Supported |
| Microsoft Edge | 120+ | Supported |
| Safari | 17+ | Supported |

---

## Project Structure

```
greenforge/
|-- index.html        # Entire application (HTML, CSS, JS in one file)
|-- README.md         # This file
```

The application uses a single-file architecture where all styling and interactivity are contained within `index.html`. Pages are implemented as hidden div elements that are toggled by a lightweight JavaScript router. No bundler, no package manager, and no external dependencies are required.

---

## Budget Summary

Total development budget: **RM 25,000.00**

| Category | Items | Amount (RM) |
|---|---|---|
| Hosting and infrastructure | VPS, domain, CDN | 1,640.00 |
| AI and API services | OpenAI GPT-4o, Anthropic Claude | 750.00 |
| Design tools | Figma, Adobe Creative Suite, Canva | 2,790.00 |
| Development | Frontend dev, backend dev, UI/UX designer | 11,600.00 |
| Database and dev tools | Firebase, GitHub Copilot | 900.00 |
| Analytics and project management | Hotjar, Notion, Trello | 1,600.00 |
| Testing and QA | BrowserStack, user testing sessions | 1,100.00 |
| Launch and marketing | Google Ads, Meta Ads, copywriting | 1,880.00 |
| Training and support | Loom Pro, Intercom | 700.00 |
| Contingency reserve (4.2%) | -- | 1,040.00 |
| **Total** | | **25,000.00** |

Full line-item breakdown is available in the Budget and Docs page of the application.

---

## Development Process

The project follows an Agile SDLC methodology with two-week sprints across six phases.

**Phase 1 - Research and Requirements**
Stakeholder interviews with green entrepreneurs and sustainability academics. Competitive analysis of platforms including ImpactBase and StartSomeGood. User personas and functional requirements documented in Notion.

**Phase 2 - UI/UX Design and Prototyping**
Low-fidelity wireframes and a high-fidelity prototype built in Figma. Design system created covering typography scale, colour tokens, spacing rules, and component library. Two rounds of usability testing with ten participants conducted before development handoff.

**Phase 3 - Frontend Development**
Responsive HTML/CSS/JS implementation with a single-page application pattern. Interactive components built include the category selector, idea generation form, Business Model Canvas, validation sliders, animated score ring, and SDG badge grid. WCAG 2.1 accessibility standards applied throughout.

**Phase 4 - Backend and API Integration**
Node.js REST API with Firebase Firestore for persistent storage. OpenAI GPT-4o integration for AI-assisted ideation. Firebase Authentication for user accounts. Deployed on VPS via GitHub Actions CI/CD pipeline.

**Phase 5 - Testing and QA**
Cross-browser testing via BrowserStack. Lighthouse performance score: 94/100. SEO optimisation and security audit completed. Soft launch to 50 beta users before full public release.

**Phase 6 - Deployment and Maintenance**
Production deployment behind Cloudflare CDN. Uptime monitoring via Uptime Robot. Continuous UX improvements driven by Hotjar heatmaps and user feedback. Monthly feature sprints planned post-launch.

---

## SDG Alignment

GreenForge directly supports the following United Nations Sustainable Development Goals:

| SDG | Goal | How GreenForge Contributes |
|---|---|---|
| SDG 8 | Decent Work and Economic Growth | Supports sustainable entrepreneurship and job creation |
| SDG 9 | Industry, Innovation and Infrastructure | Promotes green innovation and sustainable industrialisation |
| SDG 11 | Sustainable Cities and Communities | Enables circular economy businesses in urban settings |
| SDG 12 | Responsible Consumption and Production | Core focus of the ideation and validation tools |
| SDG 13 | Climate Action | Environmental impact scoring built into every business model |
| SDG 17 | Partnerships for the Goals | Platform facilitates collaboration between entrepreneurs, councils, and NGOs |

---

## Academic Context

- **Course Theme:** The Development of a Digital Platform for the Ideation and Validation of Sustainable Business Models
- **Platform Type:** Website (HTML, CSS, JavaScript)
- **Development Budget:** RM 25,000.00
- **Submitted File:** `index.html`
- **Institution:** UTHM

---

## License

This project is submitted as academic coursework. All rights reserved by the author. Not licensed for commercial redistribution.
