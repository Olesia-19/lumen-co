# LUMEN & CO. — Cursor Project Rules

## Project Overview

LUMEN & CO. is a physician-led aesthetic studio marketing website.

The current project is a static single-page website built with:

* HTML5
* CSS3
* Vanilla JavaScript
* Google Fonts
* Remote media hosted primarily on Cloudinary, with one Unsplash image

There is currently:

* no React
* no Next.js
* no Vue
* no TypeScript
* no npm/package.json
* no build step
* no component framework

The main implementation is contained in:

* `index.html`

The file currently contains the page HTML, CSS, and JavaScript.

## Core Principle

Improve the existing website incrementally.

Do not rebuild working parts of the site without a clear UX, content, or technical reason.

Do not introduce a framework, build system, or major architectural change unless explicitly requested.

The existing site is intentionally a static marketing website.

## UX Source of Truth

Before making meaningful UX or structural changes, read:

`docs/UX-SPECIFICATION.md`

The UX specification defines:

* target audience
* user needs and concerns
* business goals
* information hierarchy
* section purposes
* CTA strategy
* content priorities
* trust strategy
* responsive UX principles

Do not make UX decisions that conflict with the specification without explaining why the specification should change.

## Existing Site Structure

The current page contains:

* Navigation
* Mobile navigation
* Hero
* Trust strip
* About / Practitioner
* Treatments
* Results
* Pricing
* FAQ
* Contact / Booking
* Footer

Preserve this overall structure unless a specific UX decision requires a change.

## Design Direction

The visual direction should remain:

* calm
* premium
* professional
* trustworthy
* personal
* modern
* refined
* natural rather than trend-driven

Avoid:

* aggressive sales language
* unnecessary visual effects
* excessive animation
* clutter
* artificial-looking design
* unnecessary sections
* unnecessary UI elements
* generic template-like styling

Preserve the existing visual identity when making local improvements.

Reuse existing design patterns and classes where appropriate, including:

* `.section`
* `.section-inner`
* `.eyebrow`
* `.glass`
* `.glass-dark`
* `.btn`
* `.btn-primary`
* `.btn-ghost`
* `.btn-line`
* existing card patterns
* existing `.reveal` animation pattern

Do not create duplicate styles when an existing pattern can be reused safely.

## Content and Medical Claims

Do not invent:

* medical credentials
* certifications
* qualifications
* statistics
* patient outcomes
* testimonials
* clinical claims
* treatment guarantees
* safety claims
* before/after claims
* pricing facts

If information is missing, use an explicit placeholder or ask for the information.

Do not make medical claims stronger merely to make marketing copy sound more persuasive.

## Practitioner Trust

The practitioner section should help answer:

"Can I trust this practitioner with my face?"

Trust should be supported through information such as:

* name
* professional role
* credentials (in this conceptual demo, only clearly labelled fictional demonstration content in the credentials dialog)
* relevant experience
* treatment philosophy
* approach to natural results

Never present credentials, certification numbers, issuing organisations, or verification URLs as real. Fictional demonstration credentials must stay clearly labelled as such.

## Calls to Action

The primary business goal is consultation booking.

The primary CTA is:

"Book a Consultation"

Use consistent CTA language unless there is a specific UX reason to change it.

Avoid creating multiple competing primary CTAs.

Secondary CTAs should support the user's decision-making rather than distract from consultation booking.

## Treatments

Preserve the existing top-level treatment categories:

* Injectables
* Skin
* Body
* Laser

Do not invent additional top-level categories unless explicitly requested.

## Pricing

Pricing should be transparent and understandable.

If prices are described as "starting at", explain what can affect the final price when relevant, such as:

* amount of product used
* number of treatment areas
* practitioner assessment
* treatment complexity

The consultation should be clearly identified as complimentary/free if that is the approved business information.

Do not invent prices.

## Accessibility

Use semantic HTML where appropriate.

Maintain:

* meaningful heading hierarchy
* accessible buttons and links
* appropriate form labels
* useful alt text for meaningful images
* keyboard-accessible interactions
* visible focus states where appropriate
* sufficient text contrast
* reduced-motion support

Do not remove existing `prefers-reduced-motion` behavior without a specific reason.

## Responsive Design

Every meaningful UI change must be checked for:

* desktop
* tablet
* mobile

Do not optimize only for desktop.

Use the existing responsive system and breakpoints unless there is a clear reason to change them.

## JavaScript

Use the existing vanilla JavaScript approach.

Do not introduce a JavaScript framework for small interactions.

Preserve existing functionality unless the requested change requires modifying it.

Existing behaviors include:

* mobile navigation
* FAQ accordion
* hero video behavior
* scroll-driven hero behavior
* word reveal
* parallax
* IntersectionObserver reveal animations

When modifying JavaScript, avoid breaking unrelated interactions.

## Images and External Assets

Do not replace existing images or video merely for visual preference unless requested.

When adding or changing images:

* use appropriate `alt` text
* avoid inventing image URLs
* preserve the existing visual direction
* consider loading performance
* avoid unnecessary external dependencies

Do not add placeholder images to production content without clearly identifying them as placeholders.

## Scope Control

Make the smallest change that solves the requested problem.

Do not:

* refactor unrelated code
* rename large numbers of classes without reason
* redesign unrelated sections
* migrate frameworks
* introduce dependencies
* change the visual identity
* rewrite the entire page

A request to improve one section should normally affect only that section and its directly related styles/scripts.

## Plan Before Significant Changes

For meaningful changes involving multiple sections, complex interactions, layout restructuring, or several files:

1. Inspect the existing implementation.
2. Read `docs/UX-SPECIFICATION.md`.
3. Use Cursor Plan Mode.
4. Identify the relevant HTML, CSS, and JavaScript.
5. Explain the proposed changes.
6. Do not modify files while only planning.
7. Review the plan before implementation.
8. Implement only the approved scope.
9. Check the result on desktop and mobile.

For small changes such as:

* copy edits
* small spacing adjustments
* minor typography changes
* simple CSS fixes
* small bug fixes

Plan Mode is not required.

## Visual References

If a Figma design, screenshot, wireframe, or other visual reference is provided, treat it as the visual source of truth for the requested section.

Do not reinterpret the design unnecessarily.

Match:

* hierarchy
* layout
* spacing
* proportions
* typography
* colors
* imagery
* component placement

while maintaining responsive behavior and accessibility.

## Figma Workflow

The intended workflow is:

UX specification
→ low-fidelity wireframe
→ high-fidelity design
→ Cursor implementation plan
→ implementation
→ browser review
→ iteration

Do not skip UX reasoning by immediately generating code when a new section or significant layout change is being designed.

## Change Management

Update `docs/UX-SPECIFICATION.md` when an underlying UX decision changes, for example:

* section purpose
* information hierarchy
* user flow
* CTA strategy
* major content structure
* target-user assumptions

Do not update the UX specification for ordinary implementation details such as:

* small spacing changes
* minor font-size changes
* pixel-level alignment
* breakpoint adjustments
* small CSS refinements

## Before Finishing a Change

Check:

* requested functionality works
* existing functionality still works
* no obvious console errors were introduced
* desktop layout
* mobile layout
* accessibility basics
* responsive behavior
* visual consistency with the existing site
* no unrelated files were changed unnecessarily

After implementation, briefly report:

1. What changed
2. Which files changed
3. Any important assumptions
4. Anything that still requires manual verification
