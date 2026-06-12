# PRD — Cashin Workforce Solutions Website

*Generated with Claude (AI) from PROPOSAL.md, then reviewed and edited by Tyler.*

## 1. Overview

A three-page static marketing site for Cashin Workforce Solutions LLC, a new single-principal HR & talent acquisition consultancy serving commercial, oil & gas, and industrial businesses. The site's job is to make a brand-new one-person firm credible to corporate buyers and convert visitors into booked intro calls.

## 2. Goals

| Goal | Measure |
|---|---|
| Establish credibility with corporate executives | Visitor can identify founder's 20-year Shell background within one scroll of the About page |
| Convert interest into conversations | Every page ends in a contact CTA; booking is reachable in one click from any page |
| Look like a firm, not a freelancer | Consistent brand voice ("we"), wordmark logo, polished typography |
| Be maintainable by a non-technical owner | Static HTML/CSS, no build step, one-line Calendly swap |

## 3. Audience

Corporate executives, HR leaders, and hiring managers in commercial business, oil & gas, and industrial operations. They skim, they judge credibility fast, and they are often on a phone between meetings — mobile must be first-class.

## 4. Information Architecture

- **index.html** — Hero (value prop + stats) → Services (3) → Industries (3) → Approach (4 tenets) → About teaser → CTA
- **about.html** — Page hero → Bio + portrait → Career timeline & credentials → CTA
- **contact.html** — Page hero → Contact form | Booking / email / phone cards

Shared `styles.css`, shared header/nav/footer on all pages.

## 5. Functional Requirements

| # | Requirement | Status |
|---|---|---|
| F1 | Three pages with consistent navigation | Done |
| F2 | Semantic HTML5 (`header`, `nav`, `main`, `section`, `footer`) | Done |
| F3 | Single external stylesheet; CSS Grid + Flexbox layout | Done |
| F4 | Responsive — grids collapse to one column ≤ mobile breakpoint | Done |
| F5 | Services section lists exactly: Talent Acquisition, HR Operations, Employee Development | Done (per client feedback 6/12) |
| F6 | About page reflects verified career history (Shell 2006–2026, FSU, Certified Mediator) | Done |
| F7 | Contact form with HTML validation attributes (`required`, `type=email/tel`) | Done (composes mailto; form service is a production follow-up) |
| F8 | Calendly booking integration — popup widget, single-constant URL swap | Done (awaiting client's URL) |
| F9 | Favicon (inline SVG data URI) | Done |
| F10 | Open Graph meta tags on all pages | Done |
| F11 | Scroll-reveal transitions with `prefers-reduced-motion`/noscript fallback | Done |
| F12 | Deployed on GitHub Pages | This iteration |

## 6. Design System

- **Colors:** cream background `#F7F5F0`, dark navy `#081A2B`, blue accent (client preference: blue), copper for draft flags
- **Type:** Besley (serif, display) + Archivo (sans, UI) via Google Fonts
- **Voice:** firm "we", plainspoken, anti-buzzword ("Practical support, not theory")

## 7. Content Requirements

| Content | Source | Status |
|---|---|---|
| Services copy | Client interview + feedback call | Final |
| Founder bio & career timeline | Client's LinkedIn (with permission) | Final, client to confirm |
| Headshot | Client | Pending (styled placeholder shipped) |
| Phone / business email | Client | Pending (marked placeholders) |
| Calendly URL | Client | Pending (one-line swap in contact.html) |

## 8. Non-Goals (Out of Scope)

- CMS, blog, or testimonials (no clients yet — firm is new)
- Backend form processing (mailto now; Formspree noted as production path)
- Multi-language, analytics, SEO beyond meta tags

## 9. Acceptance Criteria

- Live on GitHub Pages with working navigation between all three pages
- Lighthouse accessibility ≥ 90
- Renders one-column, readable, no horizontal scroll at 375px width
- Client has reviewed the live URL and approved (done — feedback call 6/12, design approved unchanged)
