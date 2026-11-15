---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # A little less vertical space between homepage sections
  spacing: '4rem'

sections:
  - block: resume-biography
    content:
      username: me
      text: ''
    design:
      background:
        gradient_mesh:
          enable: true
      avatar:
        size: small
        shape: circle
  - block: markdown
    id: research
    content:
      title: 'Research'
      subtitle: ''
      text: |-
        I study how vector diversity, evolution, and ecology shape the transmission of vector-borne pathogens. My work focuses on ticks and phlebotomine sand flies, combining field research with systematics, molecular biology, and omics.

        **Interested in working together?** [Get in touch](mailto:lcsousapaula@gmail.com) to discuss collaborations, data, or student projects.
    design:
      columns: '1'
  - block: collection
    id: projects
    content:
      title: Research Themes
      text: Explore my current areas of work and collaboration.
      count: 3
      filters:
        folders:
          - projects
    design:
      view: project-summary
      columns: 1
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ''
      count: 5
      filters:
        folders:
          - publications
        exclude_featured: true
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      count: 3
      filters:
        folders:
          - events
    design:
      view: date-title-summary
      columns: 1
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      page_type: blog
      count: 3
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      offset: 0
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [0, 0, 0, 0]
---
