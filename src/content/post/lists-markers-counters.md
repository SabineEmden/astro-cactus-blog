---
title: "Reading List: CSS Lists, Markers, and Counters"
description: "I needed to refresh my memory about styling lists in CSS. This is my reading list."
publishDate: "Apr 14 2026"
tags: ["css", "frontend-mentor"]
---

I'm working on the [Tech book club landing page challenge](https://www.frontendmentor.io/challenges/tech-book-club-landing-page-fZQidjHU73) on Frontend Mentor and needed to refresh my memory about styling lists with CSS. This was my reading list:

- [Learn CSS: Lists](https://web.dev/learn/css/lists) on web.dev: A good refresher on the basics of list styling
- [CSS Lists, Markers, And Counters](https://www.smashingmagazine.com/2019/07/css-lists-markers-counters/) by Rachel Andrew for Smashing Magazine: Detailed explanations of markers and counters as more advanced list features
- [Creative list styling](https://web.dev/articles/creative-list-styling) by Michelle Barker for web.dev: A collection of different ways to style lists

:::note
I had used custom list markers before, in my [Frontend Mentor - Recipe page solution](https://github.com/SabineEmden/fm-recipe-page). That was two years ago, and I didn't recall all the details. I did, however, find the starting point for my reading list in the README.
:::

My goal was to get ideas how I could style the lists on the landing page.

The page has four unordered lists with a checkmark SVG icon as list markers. The icon is part of the image assets in the starter files. Similar to the unordered lists on the recipe page, the markers are centered vertically if the list item wraps over two or more lines.

There is also an ordered list on the landing page. Its counters are positioned above the list items and have a border.

These are all cases for the `::before` pseudo-element with custom markers using the `content` property. For the ordered list, I can use `counter(list-item)` for the generated content to add numerical markers.

The `::marker` pseudo-element has only [limited options for styling](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/::marker#allowable_properties) and cannot be positioned using flexbox or grid.

_**Coming Soon:**
I plan to write a post on how I styled the lists in my [Frontend Mentor - Tech book club landing page solution](https://github.com/SabineEmden/fm-tech-book-landing-page) when I have completed the challenge._
