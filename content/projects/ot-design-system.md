---
title: "Building OTKit: From Drift to Discipline"
slug: "ot-design-system"
summary: This is a summary.
company: "OpenTable"
main_image: "/projects/images/casestudy-otkit.png"
role: "Design Systems Lead"
timeline: "1 year"
featured: true
tags:
  - design systems
  - tokens
  - governance
  - accessibility
  - enterprise UX

params:
  featured: true          # Show in featured section on homepage
  weight: 1               # Flagship project
  showInPostList: false   # Exclude from blog timeline
---
![Design system drift across OpenTable products](/projects/images/cs-restaurant-app-lifestyle.jpg)


## Overview
OTKit is OpenTable’s design system supporting Restaurant and Diner products across iOS, Android, and web. When I took ownership, the system existed—but lacked cohesion, governance, and trust. Design drift, fragmented sources of truth, and inconsistent adoption were slowing teams down and introducing costly QA issues.

My mandate was not just to redesign components, but to **turn a drifting system into an operational platform** that teams actually relied on.

---

## The Problem
Design system drift was expensive and invisible.

Research through user surveys and 1:1 interviews revealed:
- **Three competing sources of truth** (Figma, Storybook, internal token sites)
- Visual inconsistencies across products and platforms
- Late-stage QA bugs tied directly to token and component mismatch

> We estimated the cost of drift at **~$237K/year** in inefficiency and rework.

![Design system drift across OpenTable products](/projects/images/cs-legacy-sot.png)
<p style="text-align: center; font-style: italic;">Design system drift across OpenTable products before consolidation.</p>

---

## Constraints
- Six product and platform teams shipping in parallel
- Legacy UI patterns deeply embedded in production
- Cross-platform requirements (iOS, Android, Web)

![Inconsistent, inaccessible components on web](/projects/images/cs-interface-opacity.png)
<p style="text-align: center; font-style: italic;">Inconsistent and inaccessible components on web.</p>

---

## Strategy
I focused on **foundations first**, then scaled upward:

1. **Tokens before components**
2. **Color Contrast and Typescale Accessibility**
4. **Documentation**

---

## Foundations: Tokens, Type, Icons

### Color tokens
- Audited and documented all existing colors cross-platform
- Deprecated legacy redundant colors  
- Rebuilt the color system around **accessible, semantic tokens**
- Built "mixed" light/dark theming for existing UI

This resolved cases where critical actions appeared disabled, improved cross-platform parity, and made immediate implementation possible on existing UI.

![Semantic color token architecture](/projects/images/reFdWnDzFk14EtF8.png)

Semantic vs primitive token breakdown

![Semantic color token documentation](/projects/images/cs-semantic-color-documentation.png)

Color token mapping slide
![Semantic color token migration tool](/projects/images/casestudy-otkit-colormappingtool.png)
<p style="text-align: center; font-style: italic;">Establishing semantic tokens created a single source of truth across platforms and reduced downstream inconsistencies.</p>

---

### Contextual typography
The existing type system was a one-size-fits-all scale that:
- Was not mobile-optimized
- Encouraged incorrect font usage in native apps
- Had ballooned to **39 fonts in the codebase**

![Contextual typography scales across platforms](/projects/images/casestudy-otkit-diner-ab-test.png)

**Solution**
- Introduced a contextual typography scale by platform
- Defined size, weight, and family per context
- Added support for Apple Dynamic Type

**Impact**
A/B testing showed a **+2.19% increase in diner bookings** on pages using dynamic type.

![Screenshot animation of dynamic text sizing implemented on iOS](/projects/images/casestudy-otkit-dynamic-text.gif)
<p style="text-align: center; font-style: italic;">Animation of dynamic text sizing implemented on iOS</p>


Before vs after typography scale

Desktop vs mobile context


---

### Icon system
- Introduced shape-based icon grids
- Unified keyshapes for indicators
- Centralized icon repositories across platforms
- Added SF Symbol parity for accessibility
![Animation of shape-based icon creation grid with keyshapes](/projects/images/icon_grid_animated.gif)
![Screenshot of icon creation guidelines on documentation site](/projects/images/casestudy-otkit-icons-splash.png) 

<p class="summary">This enabled a **searchable, themeable SVG system** for native and web teams.</p>

![Screenshot of searchable icon library on documentation site](/projects/images/casestudy-otkit-icon-library.png) 

---

## Brand Evolution: “Black Is the New Red”
OpenTable operates in an industry dominated by red and orange. Partnering closely with Brand, we translated a premium direction into a **tokenized theming architecture** rather than one-off visual treatments.

This enabled:
- Two new font families
- A refreshed color palette
- Visual distinction for Iconic restaurants
- Brand evolution without breaking product consistency

[Image placeholder]
![OTKit theming enables brand evolution across products](/projects/images/otkit-theming.png)

Light vs dark / mass vs iconic theme comparison

Same layout, different theme

Preferably cropped tightly

This reinforces that OTKit enabled brand evolution, not just UI cleanup.

---

## Theming in Practice
We delivered multiple system-driven themes:

### Mass Theme
- Editorial-style layout
- Two-column structure inspired by e-commerce
- Booking surfaced immediately
- Minimal concepts guiding all components

### Iconic Theme
- Full-bleed imagery
- Dark wine-inspired time slots
- Sticky, accessible booking flows
- Premium experience without sacrificing usability

---

## Outcomes & Impact
Over two years, OTKit delivered measurable ROI:

- **25% reduction in QA time**
- **50% fewer Figma libraries**
- **≈ $59K/year reclaimed** in developer time
- Unified design language across 6 teams
- Supported a full OpenTable brand refresh

[Image placeholder]
![OTKit adoption across teams and platforms](/projects/images/otkit-scale.png)

Purpose: End on scale, not pixels

Good image

System adoption slide

Multi-product usage

Platform coverage diagram

This closes the loop: foundations → application → impact.
[/image placeholder]

---

## What Made This Work
- Design ambassadors instead of enforcement
- Documentation treated as a first-class artifact
- Regular demos, office hours, and a system newsletter
- Trust built through responsiveness and follow-through

---

## Reflection
The success of OTKit wasn’t the components—it was the shift in mindset.  
The system became something teams relied on, not something they worked around.

That’s the difference between a library and a platform.
