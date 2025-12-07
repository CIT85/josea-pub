# Landscapes of the World - Layout Plan

## Site-wide common sections (observed / safe assumption)

* Header: site title/logo and top navigation
* Navigation: primary nav (links to Home, Bodies of Water, Cold Areas, Deserts, Site)
* Main Content: page-specific article or content area (heading, paragraphs, images)
* Sidebar (optional): related links, quick facts, or navigation (some pages may include it)
* Footer: copyright / small site info / contact

## Per-page visual outlines

* index.html
    * Header
        * Site title / logo
        * Primary nav
    * Main
        * Intro
        *Featured links or highlights → links to topic pages
    * Footer
* site.html
    * Header
        * Site title
        * Color Palette
    * Main
        * Site overview or purpose
        * list of pages or resources
    * Footer
* bodies_of_water.html
    * Header
        * Site title
        * Primary nav (to each section of current page)
    * Main
        * Article/section: heading → explanatory paragraphs
        * Images or examples (figures)
    * Sidebar: Links to other pages (Will only appear when hovering on them)
    * Footer
* deserts.html
    * Header
        * Site title
        * Primary nav
    * Main
        * Article/section: heading → descriptive content
        * Images / lists of desert types
    * Sidebar
    * Footer
* cold_areas.html
    * Header
        * Site title
        * Primary nav
    * Main
        * Article/section: heading → content
        * Images / Descriptions
    * Sidebar
    * Footer

(Notes: each page follows the simple pattern Header → Main (article/sections ± images) → Footer; nav is in the header for consistent site navigation.)

## Planned Flexbox and Grid Locations (concise map)

* Header (header) — display: flex
    * Files: index.html, bodies_of_water.html, deserts.html, cold_areas.html
    * Purpose: aligns header content (site title/logo and top navigation) horizontally and vertically.

* Navigation group (.nav2, strong) — display: flex
    * Files: index.html, bodies_of_water.html, deserts.html, cold_areas.html
    * Purpose: aligns the small secondary nav and the adjacent strong elements horizontally with spacing (gap) and alignment rules.

* Footer (footer) — display: flex
    * Files: all pages (including site.html)
    * Purpose: lays out footer links/text horizontally, with wrapping (flex-wrap: wrap) and gaps.

* Note: Still deciding where to use grid but not sure if my files need them.

## Standard I will follow
I will be following the commmon media query breakpoint standard.

![breakpoint-standard](../img/breakpoint-standard.png)

## My responsiveness using media queries
### 769px — 1024px (Default)
- Header (Flexbox)
  - Title (left)
  - Page Navigation Sidebar (left, now unhidden)
  - Section Navigation links (right/left)
- Introduction (Grid)
- Section Content (Left)
- Summary table (Center, after last section)
- Footer (Flexbox)
  - Nav Links (left)
  - Copyright (right)
  - Contact Page Link (left)

### 481px — 768px (Tablets)
- Header (Flexbox)
  - Title (center)
  - Page Navigation Sidebar (Top below header, unhidden)
  - Section Navigation links (right/left)
- Introduction (N/A)
- Section Content (Center)
- Summary table (Center, after last section)
- Footer (Flexbox)
  - Nav Links (left)
  - Copyright (right)
  - Contact Page Link (left)

### <481px (Phone)
- Header (Flexbox)
  - Title (center)
  - Page Navigation Sidebar (Top below header, unhidden)
  - Section Navigation links (right/left)
- Introduction (N/A)
- Section Content (Center)
- Summary table (Center, after last section)
- Footer (Flexbox)
  - Nav Links (left)
  - Copyright (right)
  - Contact Page Link (left)

### For 1025px — 1200px and 1201px and greater breakpoints
It will be the same as the default breakout but content Increase in size to keep them visible. There might be changes to some content.