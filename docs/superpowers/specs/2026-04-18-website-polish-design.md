# Website Polish Design Spec
**Date:** 2026-04-18
**Scope:** Full polish pass on nestor-sun.github.io — refining the existing dark theme without structural changes.

---

## Context

Single-page academic portfolio for Dr. Mingwei Sun (Assistant Professor, Information Systems, UT Arlington). Dark near-black theme with gold accents, Poppins font, sidebar layout. Primary audience: academics/hiring committees + industry collaborators. Goal: make the site feel polished and professional, not like an unfinished template.

---

## Section 1: Sidebar

- Profile photo grows from 80px → 160px, centered
- Gold ring border: `outline: 3px solid var(--orange-yellow-crayola)` with a small offset gap
- More breathing room below photo (name + title spacing)
- CV becomes a gold-outlined button element (not underlined plain text), placed just below bio on Home page
- Social links (LinkedIn, GitHub, Scholar) get `target="_blank" rel="noopener noreferrer"`

## Section 2: Navigation

- Navbar becomes sticky — stays at top of content area while scrolling
- Clicking a nav item smoothly scrolls to top of that section (no hard jump)
- Active nav item: thicker, more visible gold underline

## Section 3: Research / Paper Entries

- Each paper entry: `border-left: 3px solid var(--orange-yellow-crayola)` + left padding
- Venue/status line below co-authors in smaller muted color (e.g. "Major Revision at Information Systems Research")
- Paper links (SSRN, DOI, PDF) rendered as small pill badges — gold outline, hover fills gold
- Hover on paper entry: subtle background highlight

## Section 4: News Section

- Visual timeline: thin gold vertical line on left, small gold dot per entry
- No dates shown

## Section 5: Cleanup & Micro-polish

- Remove dead modal code (~lines 411–437, unused testimonials modal)
- Remove large commented-out blocks (skills bars section, etc.)
- Fade-in animation on section load: opacity 0→1 + slight translate-up, ~0.3s ease
- Consistent spacing pass across sections
- All external links: `target="_blank" rel="noopener noreferrer"`

---

## Out of Scope

- Layout or structural changes
- Adding new sections or content
- Changing color palette or font
