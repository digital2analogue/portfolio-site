+++
title = "Building OpenTable's Design System"
date = 2023-01-01T08:30:00-07:00
summary = "Brief description of your project"
draft = true
main_image = "/projects/images/casestudy-otkit.png"
categories = ["casestudy"]  # optional
tags = ["tag1", "tag2"]  # optional

[params]
  featured = true  # Show in featured section on homepage
  weight = 5  # Order in featured section (lower = first)
  showInPostList = false  # Show in timeline lists alongside blog posts

+++

# Crafting a Unified Product Identity

## Background
OpenTable experienced a productivity bottleneck: product teams were spending ~25% more time than necessary due to time-consuming design reviews and UI inconsistencies. Engineers and designers were frustrated by unclear guidelines and scattered style guides.

## Problem
- Unify product UIs under a scalable design system.
- Set standards for color, typography, spacing.
- Encourage adoption by Diner & Restaurant design and engineering teams.

## Solution & Impact
Created a foundational design system, increasing cross-functional team efficiency in product development.

- Enhanced visual consistency and quality across apps.
- Reduced design QA time by ~25% with clear guidelines.
- Improved Figma workflow: Streamlined designer/developer workflows with variable support and easier theming.

## Tools
- Google surveys
- Figma
- Airtable
- JIRA

## Team
- 1 UX designer
- 1 developer
- 4 in-rotation LOB designers & platform engineers

## My Role
- UI/UX design
- UX research
- Workshop facilitator
- Project & Roadmap management

## Timeline
- Overall: 1 year
- Discovery & Research: 2+ weeks
- Design & testing: 6 months

## Sections
1. User research  
2. Creating the vision  
3. Foundations  
4. Adoption & Impact  
5. Learnings  

---

# User research

## Research surveys
### Establishing a baseline—where are we now?
We established research strategy, focusing on understanding challenges faced by design, product, and engineering teams.

**Fragmented Design**
- Design, Product & Engineering silos led to inconsistencies.
- Survey (37 responses) revealed designers & engineers spent significant time on late-stage design QA.
- Research confirmed the need for a central design system.

*Our first OTKit survey*

### Time spent creating one-off components
- **100%** of iOS designers said they were creating new or one-off components often or occasionally  
  vs  
- **60%** of web designers across both Restaurant & Diner teams who answered the same

**Insight:** iOS teams suffered the most in creating one-off components compared to web. This made sense given we did not have a Figma UI Kit or Storybook web equivalent for iOS.

### Time spent clarifying styling during release
- **4–8x** — 75% of restaurant web designers  
  vs  
- **0–3x** — 100% of Diner web designers

**Insight:** Cross-functional Restaurant teams were spending a lot more time clarifying our style guide with designers, which added more meetings and work time toward the end of a release cycle.

## Interviews and brainstorms
Remote tools used: Surveys, 1:1 interviews, Figjam, Dovetail

During the discovery phase of the project, we conducted user interviews and ran remote collaborative problem/solution brainstorming sessions. We prepared a sticky exercise with 4 open-ended problems influenced from our DS survey, and had designer and engineer stakeholders put down possible solutions, then affinity map them as a group to find common themes across all products.

The main insight from the interviews was clear: designers and engineers often had the same problem. Unclear, inconsistent sources of truth added extra workload during projects.

*Remote Problem/Solution exercise with designers & engineers*

## Consolidating research

### High-level
Most folks knew what colors and styles to use, but much of OpenTable's style guide lived in designers' heads instead of being clear and centralized.

### Specific
The core workhorse parts of our product components, and therefore the ones that were the most outdated, were the ones causing the most issues with needing to de-scope when shipping new feature work. We had an "interface" debt that we rarely paid off.

## Multiple sources of truth causing confusion
At the time of audit, OpenTable had multiple sources of truth that lived in different places and were often not in parity with one another: one tokens github, two Storybook component sites, Figma (which was often not in sync with coded components), and multiple UI Kits built by different teams in Figma.

---

# Creating the design system vision

## Problem
We knew a lot about the velocity issues teams were having with not having a clear source of truth, but, how were we going to tackle it?

## Solution
Create a vision deck for the design system solution and present to product leadership. Include user research, industry case stories, roadmap, and resourcing needs.

### Why do we need a design system?
- User research summary
- Industry case studies on impact and ROI of implementing a design system

### What are we going to do?
- Build out foundational tokens
- How should we resource the DS team now? In the near-future, in the long-term?

### What metrics we'll use to determine success
- Surveys, team interviews, the rotating OTKit Ambassadorship
- KPIs and/or OKRs: are we doing projects that align with our OTKit system principles?

---

# Foundations

## Color

### Background
OpenTable's existing style guide used non-semantic color tokens, following our style guide, which existed across all products.

We also had many legacy colors in our Restaurant products that needed updating. Our challenge was: how might we migrate from this non-semantic existing system to a semantic color system in the easiest way possible for adoption?

### Foregrounds, Backgrounds, Borders
We began by documenting the obvious—what do we already know? We knew what we used for links, buttons, disabled elements, page backgrounds, and more so we began with that. Using our product audit, we found where we did and didn't have consistencies, like disabled text. We also did contrast checks with every color, optimizing to pass AA contrast accessibility with our icons and text on top of colors.

*Color token combinations in light and dark themes*

### Feedback, extensible color palettes, and dark mode
The iteration we had after our first slice was adding an extended color palette for our accent colors—colors that are less often used in our UI and have non-semantic meanings. For instance, colors used in data visualizations, or custom statuses. We also better optimized accent colors' contrast in our dark theme after getting product feedback that they needed to be brighter.

*OTKit accent colors*

### Project challenge: Table statuses
One project in particular which helped as a real product use case for an extended palette was Table Statuses. This project needed 10 new statuses, shown with color and icon, on the floor plan. Restaurants needed to read the statuses quickly, be able to differentiate between colors, and associate each color with a table status.

### Team collaboration
The design system team collaborated with product design on a way to support these new statuses. Initially the proposal was 10 new colors to support each new status, including interactive colors for buttons using the table statuses.

### Solution: win-win
Using the existing accent colors, we satisfied project requirements and reduced the number of proposed new colors from ten to only two—lemon and lime. We also used opacity to support interactive color, without having to add additional new color tokens but still support the product team's implementation in a timely manner, with a note to follow-up on the design system debt in our next
