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
  - block: markdown
    content:
      title: 'Welcome to ISLa'
      subtitle: ''
      text: |-
        The Intelligent Systems Lab (ISLa) research group aims at developing methodological and applied research in Artificial Intelligence, Machine Learning and data analysis for intelligent systems. 

        The methodologies investigated range from reinforcement learning and planning under uncertainty to multi-agent coordination, probabilistic modeling, and statistical data analysis. The application domains range from robotics and industry 4.0 to cybersecurity and cyber physical systems. 

        The group participates in national and international projects and collaborates with Italian and foreign research centers. We are part of the Department of Computer Science at the University of Verona.
    design:
      columns: '1'
      
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
    id: events
    content:
      title: Recent & Upcoming Events
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
      page_type: blog
      count: 10
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
      view: card
      spacing:
        padding: [0, 0, 0, 0]
---
