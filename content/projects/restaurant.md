+++
title = "Modernizing OpenTable's Restaurant Platform"
date = 2023-01-01T08:30:00-07:00
summary = "Brief description of your project"
draft = false
main_image = "/projects/images/casestudy-otkit.png"
categories = ["casestudy"]  # optional
tags = ["tag1", "tag2"]  # optional

[params]
  featured = true  # Show in featured section on homepage
  weight = 2  # Order in featured section (lower = first)
  showInPostList = false  # Show in timeline lists alongside blog posts

+++


## Background
OpenTable's Front of House app is the face of a restaurant's hospitality. It's crucial for operational success: for guest information, for takeout, for table management, and reservations. This makes having a solid, usable, and information-dense user interface critical.

The challenge: how do you modernize something so sensitive to your users’ everyday workflows?

---

## Problem
OpenTable's reservation details experience was the result of years of accumulated product features centralized into one area. The issue wasn’t functionality—it was visual and structural debt.

- Heavy legacy styling made the interface feel dated
- UX improvements were difficult due to fragmented engineering ownership
- Multiple teams owned different parts of the experience
- The UI felt cobbled together and hard to evolve

Design Systems recognized the need to partner with Product to modernize the visuals **without sacrificing UX density**, which restaurant teams rely on.

---

## Solution
We modernized the Front of House app through several key improvements:

- Deprecated legacy fonts and colors
- Created new, scalable components for reservation details
- Introduced mixed light/dark theming with a path to full theming support
- Leveraged design system tokens, icons, and typography

These updates allowed us to refresh large areas of the UI quickly while laying the groundwork for a future brand refresh.

---

## Tools
- Figma  
- UserResearch.com  
- Pen and paper  

---

## Team
- 3 UX designers  
- 6 developers  
- 2 project managers (Hospitality and TMS)  
- Restaurant users  

---

## My Role
- Design System Lead  
- Workshop facilitator  
- Design System QA  

---

## Timeline
- **Overall:** 8+ weeks  
- **Discovery & Research:** 2+ weeks  
- **Design & Testing:** 8 weeks  

---

## My Design Process
1. Definition  
2. Redefining reservation details  
3. Modernization  
4. Scaling the brand refresh  
5. Next steps  
6. Conclusion  

---

## Defining Key Objectives
During discovery, Design Systems partnered with two product designers specializing in Hospitality and Table Management Services to explore web and native patterns for critical front-of-house workflows.

Key focus areas:
- Reservation details and guest profiles
- Migration to design system tokens
- Color theming updates
- Typography updates
- Icon updates

The goal was to modernize the UI while improving information density, readability, and visual appeal—without hiding critical restaurant data.

---

## Redefining Reservations

### Information Architecture & User Research
To align the IA with restaurant workflows, we conducted six remote card-sorting sessions using FigJam. These helped us identify intuitive groupings for reservation and guest profile information.

We landed on three primary categories:
- **Guest profile:** contact info, allergies, VIP status
- **Visit information:** occasion, notes, seating requests
- **Primary actions:** table assignment, status, messaging

---

### Modular Design Strategy
Using Figma, FigJam, and Zoom, we explored:
- Condensed information layouts (loyalty, social, payments)
- Patterns for detailed views (panels, modals, half-sheets)
- Platform differences between web and mobile
- Modular components reusable across the product

---

### Perfecting the “Just Right” UI
We proposed a card-based layout with expandable detailed views to balance information density and clarity.

- Expandable cards for progressive disclosure
- Subtle motion using ease-in / ease-out transitions
- Visual hierarchy tuned for dense operational workflows

---

## Modernization

### Updating Legacy Components with the Design System
With teams distributed across San Francisco and Melbourne, async collaboration was essential.

Thanks to design system documentation:
- Engineers could update components independently
- Live demos were shared for QA
- Tokens and guidelines reduced back-and-forth
- Office hours handled edge cases

Compared to previous work in this area without a design system, the efficiency and collaboration gains were substantial.

---

### Light, Dark, and Mixed Theming
Because the Restaurant app was not originally designed for full theming, we introduced mixed theming alongside light and dark modes—with a plan to move to pure modes later.

As one iOS developer put it:
> “We got dark mode for free.”

---

## Updating Typography

### Leading with Accessibility
We used the Restaurant iOS app as a pilot for testing dynamic text support.

- Allowed restaurants to adjust text size on dense screens
- Tested on Restaurant first
- Ran an A/B test on the Diner iOS app with strong positive results

---

### Slicing Large Visual Changes
To reduce risk, we shipped typography changes in phases:
1. Migrate from Source Sans Pro to SF Pro Text (same sizing)
2. Validate layout and fix issues
3. Update to OTKit type sizing
4. Run bug bashes across the app

---

## Updating Iconography

### A Searchable, Centralized Icon Library
We consolidated multiple icon repositories into a single, searchable source of truth.

- Improved consistency
- Simplified legacy page updates
- Enabled faster design and engineering workflows

---

## Refreshing the OpenTable Brand

### Design System as a Tool for Change
In late 2023, OpenTable launched a brand refresh tied to its anniversary, targeting both iconic and general restaurant audiences.

The refresh was built directly on design system foundations.

---

### Black Is the New Red
The brand refresh introduced:
- Two new variable font families: **Haffer** and **Nantes**
- A new color palette layered on top of semantic tokens

Finding a new “workhorse” font for dense Restaurant interfaces was a significant challenge, but essential for long-term scalability.

---

## Redefining Restaurants
Exploration included:
- Research across 15+ competitors
- 10 key patterns and 12 key statistics identified
- 22+ color logic concepts explored
- 2 scalable, accessible proposals distilled

---

## Next Steps: Migrating to the New Brand
With the brand defined:
1. Diner engineering adopted OTKit semantic tokens
2. Updates were sliced into web and native releases
3. Feedback informed iteration and rollout strategy

---

## Learnings

### Change Is Constant
Modernizing to semantic tokens while launching a brand refresh was a communication challenge—especially remotely. Shared token language made cross-team collaboration far more effective.

---

### Communicating in a Remote World
Working across the UK, Melbourne, and the US required:
- Async Loom videos
- Slack communication
- Recorded demos
- Design system office hours

Sustainable async workflows were key.

---

### Balancing Blue-Sky Ideas with System Constraints
Great design systems support exploration without blocking innovation. Allowing brand concepts to breathe—while guiding them toward scalable, technical realities—is a critical soft skill.

---

## Conclusion
Thank you for reading my case study!
