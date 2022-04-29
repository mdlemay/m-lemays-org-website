---
# An instance of the Pages widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: pages

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 140

title: Recent Posts
subtitle:

content:
  # Filter on criteria
  filters:
    folders:
      - post
    tag: ''
    category: ''
    publication_type: ''
    author: ''
    exclude_featured: false
    exclude_future: false
    exclude_past: false
  # Choose how many pages you would like to display (0 = all pages)
  count: 5
  # Choose how many pages you would like to offset by
  offset: 0
  # Page order: descending (desc) or ascending (asc) date.
  order: desc

design:
  # Choose a view for the listings:
  view: compact
  columns: '2'
---
I post a mix of professional content and home/personal content on my website, and I categorize my posts accordingly. Separate RSS/Atom feeds are generated for each of those categories, and there is also a combined feed:
* [Professional](https://m.lemays.org/category/work/index.xml) ([archive](https://m.lemays.org/category/work/))
* [Home/personal](https://m.lemays.org/category/home/index.xml) ([archive](https://m.lemays.org/category/home/))
* [Combined](https://m.lemays.org/index.xml)
