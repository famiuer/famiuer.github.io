---
title: ''
summary: ''
date: 2022-10-24
type: landing

aliases:
  - /about/
  - /about.html

design:
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: View CV
        url: /cv/
      headings:
        about: About
        education: Education
        interests: Interests
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: markdown
    content:
      title: Research Focus
      subtitle: ''
      text: |-
        My current work is in offshore wind energy and the marine environment.

        I am especially interested in numerical hydrodynamics, wave modeling,
        fluid-structure interaction, and statistical methods such as extreme value analysis.

        If you would like to collaborate or discuss related topics, feel free to contact me.
    design:
      columns: '1'

  - block: collection
    id: papers
    content:
      title: Publications
      filters:
        folders:
          - publications
    design:
      view: citation

  - block: collection
    id: news
    content:
      title: Recent Posts
      page_type: blog
      count: 6
      filters:
        exclude_featured: false
        exclude_future: false
        exclude_past: false
      order: desc
    design:
      view: card
      spacing:
        padding: [0, 0, 0, 0]
---
