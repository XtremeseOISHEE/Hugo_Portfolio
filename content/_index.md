---
title: ''
date: '2026-11-24'
type: landing
design:
  spacing: 5rem
sections:
- block: resume-biography-3
  content:
    username: admin
    button:
      text: Explore my CV
      url: cv/
  design:
    css_class: portfolio-hero
- block: collection
  id: projects
  content:
    title: Selected research & engineering
    count: 6
    text: Evidence-grounded AI, wearable sensing, and software built around real problems.
    filters:
      folders:
      - project
      featured_only: true
    sort_by: Weight
    sort_ascending: true
  design:
    view: article-grid
    columns: 2
    fill_image: false
- block: markdown
  content:
    title: Research in progress
    text: 'My multi-hop XAI work investigates whether each reasoning step is supported
      by retrieved clinical evidence. BeyondFall explores wearable fall detection
      with patient-initiated episode logging. Both are research prototypes; manuscripts
      are unpublished or in preparation.


      [Read about my research](research/) · [Get in touch](contacts/)'
  design:
    columns: '1'
---
