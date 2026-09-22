# LUMEN & CO. — UX Specification

## 1. Project Overview

LUMEN & CO. is a physician-led aesthetic studio focused on helping clients achieve natural-looking improvements through personalized aesthetic treatments.

The website should communicate:

* professional credibility
* safety and trust
* natural-looking results
* personalized treatment
* calm, premium service
* no unnecessary procedures
* no pressure to purchase treatment

The website should feel refined and trustworthy rather than aggressive, trendy, or overly commercial.

---

# 2. Target User

## Primary Audience

Women approximately 30–50 years old who are beginning to notice changes associated with aging and are considering aesthetic treatments.

They want to look refreshed and improved while still looking like themselves.

They are not primarily looking for dramatic transformation.

## User Mindset

The user may be interested in treatment but is cautious.

She may be asking:

> "Can I trust this practitioner with my face?"

She wants enough information to feel comfortable booking a consultation.

---

# 3. User Concerns

The website should address the user's major concerns:

* Is the practitioner properly qualified?
* Does the practitioner have enough experience?
* Will the result look natural?
* Will I be pressured into unnecessary treatment?
* Could the treatment make me look worse or unnatural?
* Will someone recommend treatments I do not actually need?
* Will my consultation feel rushed?
* How much will treatment actually cost?
* What treatment might be appropriate for me?

These concerns should be addressed through information, hierarchy, evidence, and tone rather than aggressive persuasion.

---

# 4. User Goals

## Functional Goal

Understand the clinic, practitioner, treatments, results, and pricing well enough to decide whether to book a consultation.

## Emotional Goal

Feel:

* safe
* informed
* respected
* understood
* confident enough to take the next step

## Primary User Action

Book a consultation.

---

# 5. Business Goal

The primary business goal of the website is:

**Book a Consultation**

The website should move the user naturally toward consultation booking without making every section feel like a sales pitch.

---

# 6. Global UX Principles

## 6.1 Trust Before Persuasion

The user should receive evidence and relevant information before being asked to commit.

Trust should come from:

* practitioner information
* credentials
* experience
* treatment philosophy
* realistic results
* transparent pricing
* clear consultation information

Avoid unsupported claims.

## 6.2 Natural Results

The brand should consistently communicate a preference for natural-looking results.

Avoid language or visual direction suggesting:

* dramatic transformation
* exaggerated beauty standards
* trend-driven procedures
* "perfect" faces
* guaranteed outcomes

## 6.3 No Pressure

The website should not make the user feel pushed into treatment.

The consultation should be presented as an opportunity to discuss options rather than an obligation to purchase.

## 6.4 Clarity Over Complexity

The user should be able to understand:

1. What the clinic does
2. Who the practitioner is
3. What treatments are available
4. What results look like
5. What treatment may cost
6. What happens next

Do not add complexity without a clear user benefit.

## 6.5 Progressive Confidence

The page should gradually increase user confidence:

**Awareness → Trust → Understanding → Evidence → Transparency → Action**

---

# 7. Page Structure

The current page structure is:

1. Hero
2. Trust Strip
3. Practitioner / About
4. Treatments
5. Results
6. Pricing
7. FAQ
8. Booking / Contact
9. Footer

The existing structure should be preserved unless a specific UX problem justifies a change.

---

# 8. HERO

## Purpose

Immediately communicate:

* what LUMEN & CO. is
* the core value proposition
* the desired emotional outcome
* an initial trust signal
* the next step

The Hero should make the user understand the brand within a few seconds.

## Primary User Question

"Is this a clinic/practitioner I might trust?"

## Information Hierarchy

Recommended hierarchy:

1. Brand / category context
2. Main headline
3. Supporting value proposition
4. Primary CTA
5. Trust / credibility signal
6. Supporting visual

## Primary CTA

**Book a Consultation**

## Visual Direction

The existing Hero uses a large visual/video background.

The background should support the content rather than compete with it.

Text must remain readable over the visual.

## Acceptance Criteria

The Hero should:

* communicate the clinic's positioning quickly
* make the primary CTA obvious
* communicate a natural, premium aesthetic
* establish an initial trust signal
* remain readable on mobile
* maintain visual hierarchy over the background video

Do not add unnecessary content to the Hero.

---

# 9. TRUST STRIP

## Purpose

Provide quick supporting trust signals immediately after the Hero.

The trust strip should reinforce credibility without becoming a wall of text.

## UX Principle

Trust signals should support the user's decision rather than overwhelm her.

Use only verified information.

Do not invent certifications, memberships, awards, or statistics.

---

# 10. PRACTITIONER / ABOUT

## Purpose

This is one of the most important trust sections.

It should answer:

> "Can I trust this practitioner with my face?"

## Information Hierarchy

Recommended order:

1. Practitioner photo
2. Name
3. Professional role
4. Verified credentials
5. Relevant experience
6. Philosophy / approach
7. Credential Verification
8. Principles
9. CTA

## Credential Verification

The Practitioner section should include a secondary control:

**View credentials →**

Placement:

* directly after the practitioner introduction paragraph
* before the philosophy/principles cards

Purpose:

* support the trust question “Can I trust this practitioner with my face?”
* give the user structured professional-background information without leaving the page
* keep this supporting evidence visually secondary to the primary consultation CTA

Interaction:

Lumen & Co. is a conceptual/demo website and Dr. Elena Marsh is a fictional practitioner. Clicking **View credentials →** opens an on-page credentials dialog. It must not navigate to another page, an external verification URL, or a PDF.

The dialog should present clearly labelled fictional demonstration content only (name, demonstration certification/training titles, and stated clinical experience). It must not include credential IDs, registration numbers, issuing organisations presented as real, verification buttons, or any implication that the credentials can be independently verified.

A subtle note must appear at the bottom of the dialog:

“Practitioner credentials shown are fictional and for demonstration purposes only.”

The dialog should feel like a calm extension of the site, not an official medical-regulatory certificate.

Accessibility:

* treat the overlay as a modal dialog (`role="dialog"`, `aria-modal="true"`, accessible title)
* include a close control named “Close credentials”
* close on Escape and on click outside the dialog
* move focus into the dialog on open and restore it to the trigger on close
* prevent background page scrolling while open

The trigger should remain visually secondary to **Book a Consultation**.


## Existing Content Direction

The section may communicate principles such as:

* no unnecessary treatments
* no chasing trends that compromise natural expression
* no rushed consultations

These principles are important because they address the user's concerns directly.

## Primary CTA

**Book a Consultation with Dr. Elena**

Use the real practitioner name and credentials only when verified.

## Acceptance Criteria

The section should:

* humanize the practitioner
* establish professional credibility
* explain the practitioner's approach
* communicate the preference for natural results
* reduce fear of being pressured into unnecessary treatment
* provide a clear next step

---

# 11. TREATMENTS

## Purpose

Answer:

> "What does the clinic offer?"

The existing treatment categories should remain:

* Injectables
* Skin
* Body
* Laser

Do not create additional top-level categories unless there is a clear UX reason.

## UX Principle

The user should be able to quickly understand the treatment areas without needing to read large amounts of text.

Treatment descriptions should explain the purpose/value of each category rather than becoming overly technical.

## CTA

A consultation CTA may be used after the section if appropriate.

The CTA should help users who are interested but uncertain about which treatment is right for them.

---

# 12. RESULTS

## Purpose

Provide visual evidence of the clinic's approach and outcomes.

The user should be able to understand:

* what treatment was performed
* the type of result
* relevant context
* that results are individual

## Existing Structure

Preserve the existing results gallery and before/after presentation unless there is a specific UX problem.

Do not redesign the gallery unnecessarily.

## Contextual CTA

After the results section, a contextual CTA may be used:

**Considering a similar result? Book a consultation to discuss what may be appropriate for you.**

Do not imply that the same result is guaranteed.

## Disclaimer

Results should remain appropriately contextualized.

Do not present individual outcomes as guaranteed results.

---

# 13. PRICING

## Purpose

Reduce uncertainty around cost.

Pricing should feel transparent rather than intentionally vague.

## "Starting At" Pricing

If a treatment is displayed as:

**Starting at €X**

the page should explain what can affect the final price.

Relevant factors may include:

* amount of product used
* number of treatment areas
* practitioner assessment
* treatment complexity

Only use factors that are actually applicable to the treatment.

## Consultation

If the consultation is complimentary/free, this should be clearly communicated.

The user should understand that the final treatment recommendation and price can be confirmed during consultation.

## Acceptance Criteria

The pricing section should answer:

* What is the starting price?
* Why might the final price be different?
* Is consultation free?
* When will the final treatment plan and price be confirmed?

Do not invent prices or pricing rules.

---

# 14. FAQ

## Purpose

Resolve remaining objections before booking.

The FAQ should answer practical and emotional concerns.

Potential questions include:

* What happens during the consultation?
* Will I be pressured to book treatment?
* How do I know which treatment is right for me?
* How do you approach natural-looking results?
* What qualifications does the practitioner have?
* How is the final treatment price determined?
* How long does a consultation take?
* What should I expect after treatment?

Only include questions that can be answered accurately.

---

# 15. BOOKING / CONTACT

## Purpose

Convert established trust into action.

By this point the user should already understand:

* what the clinic does
* who the practitioner is
* what treatments are offered
* what results look like
* how pricing works

The Booking section should make the next step feel simple and low-pressure.

## Positioning

The existing direction:

> Let's talk before we treat.

This supports the brand's non-pressure approach.

## Primary CTA

**Book a Consultation**

## Supporting Message

The consultation should be presented as a conversation and assessment, not as an automatic commitment to treatment.

If accurate, communicate:

* complimentary consultation
* no obligation
* personalized assessment

Do not make claims that are not operationally true.

---

# 16. NAVIGATION

Navigation should allow users to move quickly between the main information areas.

Primary navigation anchors:

* About
* Treatments
* Results
* Pricing
* FAQ
* Contact

The primary CTA should remain visually distinct:

**Book a Consultation**

Navigation should remain usable on mobile.

---

# 17. MOBILE UX

Mobile is not simply a smaller desktop layout.

The mobile experience should preserve:

* information hierarchy
* CTA visibility
* readable text
* comfortable spacing
* touch-friendly controls
* usable navigation
* understandable content order

The primary CTA should remain easy to find.

Animations should respect `prefers-reduced-motion`.

---

# 18. VISUAL DESIGN DIRECTION

The visual design should communicate:

* premium
* calm
* clinical credibility
* warmth
* sophistication
* natural beauty

The design should avoid:

* aggressive luxury clichés
* excessive glassmorphism
* excessive animation
* clutter
* overly decorative UI
* generic stock-clinic aesthetics
* visually exaggerated beauty imagery

Existing visual patterns should be reused where appropriate.

---

# 19. CONTENT PRINCIPLES

Copy should be:

* clear
* concise
* confident
* warm
* professional
* non-judgmental
* non-aggressive

Avoid:

* exaggerated promises
* fear-based sales
* guaranteed outcomes
* unnecessary medical jargon
* artificial urgency
* manipulative conversion language

---

# 20. ACCESSIBILITY

The site should maintain:

* semantic HTML
* logical heading hierarchy
* keyboard accessibility
* accessible buttons and links
* form labels
* meaningful alt text
* readable contrast
* reduced-motion support

Accessibility should be considered during implementation rather than added only at the end.

---

# 21. RESPONSIVE UX

Every significant design decision should be evaluated across:

* desktop
* tablet
* mobile

Important visual relationships should remain intact across screen sizes.

Do not simply shrink desktop layouts.

---

# 22. DESIGN AND IMPLEMENTATION WORKFLOW

The intended workflow for significant UX changes is:

### Step 1 — UX Decision

Define:

* user problem
* user goal
* business goal
* information hierarchy
* desired action

### Step 2 — Low-Fidelity Wireframe

Focus on:

* structure
* hierarchy
* content placement
* spacing relationships
* CTA placement
* responsive structure

Do not focus on final colors or decorative styling.

### Step 3 — High-Fidelity Design

Define:

* typography
* colors
* imagery
* exact spacing
* buttons
* borders
* shadows
* visual details
* responsive behavior

### Step 4 — Technical Plan

Use Cursor Plan Mode for meaningful implementation work.

The plan should identify:

* relevant HTML
* relevant CSS
* relevant JavaScript
* implementation approach
* potential side effects

### Step 5 — Implementation

Use Cursor Agent to implement the approved plan.

### Step 6 — Browser Review

Check:

* desktop
* mobile
* interaction
* accessibility
* visual consistency

### Step 7 — Iteration

Fix issues based on actual browser review.

---

# 23. UX SPECIFICATION MAINTENANCE

This document is a source of truth for meaningful UX decisions.

Update it when there is a change to:

* target audience
* user problem
* user goal
* business goal
* information hierarchy
* section purpose
* CTA strategy
* major content structure
* user flow

Do not update this document for every implementation detail.

The following normally do NOT require a UX specification update:

* changing 48px spacing to 44px
* adjusting a font size
* changing a breakpoint
* fixing alignment
* changing a border radius
* correcting a CSS bug
* adjusting animation timing

The specification describes **why and what**.

The implementation describes **how**.

---

# 24. CORE UX PRINCIPLE

The goal is not to redesign every part of the website.

A successful UX decision may be:

> "This section already works. Keep it."

Changes should be made when they solve a real user or business problem.

The website should become clearer, more trustworthy, and easier to use — not simply more complicated.
