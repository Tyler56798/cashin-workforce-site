# Cashin Workforce Solutions — Client Website

**Live site:** https://tyler56798.github.io/cashin-workforce-site/

## The Client

Mike, a family friend in Houston who spent 20+ years leading HR and talent acquisition at Shell and just founded his own consultancy, Cashin Workforce Solutions LLC. He needed a site that makes a brand-new one-person firm look credible to corporate executives.

## The Site

Three pages — Home, About, Contact — built with semantic HTML and a single shared stylesheet (CSS Grid + Flexbox, responsive, scroll-reveal transitions, Google Fonts, Open Graph tags). The contact page has a validated contact form and a Calendly booking integration that goes live the moment the client supplies his scheduling link.

Built from a real client interview, then revised after a feedback call where the client approved the design and finalized his three core services (Talent Acquisition, HR Operations, Employee Development). His bio and career timeline come from his LinkedIn profile, used with permission.

## Project Docs

- [PROPOSAL.md](PROPOSAL.md) — client brief from the interview
- [PRD.md](PRD.md) — product requirements doc generated from the proposal with AI
- `layout-sketch.jpg` — hand-drawn layout before any code

## What I Learned

The biggest surprise was the client feedback: I think the site is still a bit basic and has room to grow, but Mike was genuinely happy with it and asked for zero design changes. That taught me that the client's taste and the developer's taste are two different things — what reads as "basic" to me read as "clean and professional" to him, and his judgment is the one that counts.

I also leveled up how I work with AI compared to my earlier projects: instead of asking for code and pasting it in, I gave it real context (a client brief, his actual LinkedIn career history, specific feedback from our calls) and reviewed what came back. The result felt like directing the work rather than receiving it. On the technical side, I got comfortable with CSS Grid layouts that collapse for mobile, `clamp()` for fluid type sizes, and using IntersectionObserver for scroll-reveal effects with a `noscript` fallback so the page still works without JavaScript.
