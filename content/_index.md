---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
#      button:
#        text: Download CV
#        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        experience: ''
       
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: sm # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    id: research
    content:
      title: 'Research'
      subtitle: ''
      text: |-
        I study how vector diversity, evolution, and ecology shape the transmission of vector-borne pathogens. My work centers on ticks and phlebotomine sand flies, combining field and ecological research with systematics, molecular biology, and omics.

        ### Tick genomics and systematics

        Reference genomes and phylogenomic approaches can help resolve species boundaries and improve the tools available for tick research.

        ### Sand fly diversity and omics

        I use systematic and molecular approaches to investigate phlebotomine diversity, evolutionary relationships, and the biology of medically important species.

        ### Vector–pathogen interactions

        I am interested in how vector, pathogen, and vertebrate-host relationships influence transmission, and how molecular methods can strengthen surveillance.

        **Interested in working together?** [Get in touch](mailto:lcsousapaula@gmail.com) to discuss collaborations, data, or student projects.
    design:
      columns: '1'
  - block: collection
    id: projects
    content:
      title: Research Themes & Projects
      text: See current areas of work and collaboration.
      filters:
        folders:
          - projects
    design:
      view: article-grid
      fill_image: false
      columns: 3
      show_date: false
      show_read_time: false
      show_read_more: true
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
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - events
    design:
      view: card
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 10
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
---
