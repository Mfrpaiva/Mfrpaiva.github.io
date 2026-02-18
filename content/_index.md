---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-01-05
type: landing

design:
  # Default section spacing
  spacing: '0'

sections:
  # Developer Hero - Gradient background with name, role, social, and CTAs
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Hi, I'm"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "Catalyzing"
        strings:
          - "reactions"
          - "people"
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: View Info and Works
          url: "#projects"
          icon: arrow-down
        - text: Get In Touch
          url: "#contact"
          icon: envelope
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]

# Biography Section
  - block: markdown
    id: biography
    content:
      title: Biography and scientific vision
      text: |
          <div style="text-align: justify;">
            "Catalyzing people and reactions" is more than a motto – it is the principle that has guided both my scientific journey and my way of engaging with others. In chemistry, catalysis accelerates transformation without being consumed. In life, I strive to play a similar role: enabling progress, fostering collaboration, and empowering those around me to go further than they imagined possible. My academic path reflects this dual commitment to scientific advancement and collective growth. I hold a PhD in Materials Chemistry from the Université de Lille (France), awarded within the PEARL i-site / Marie Skłodowska-Curie Actions excellence framework and recognized with the European Doctorate Label. My doctoral research integrated catalysis and combustion toward advanced lignocellulosic biomass valorization, combining fundamental understanding with sustainable technological applications. Originally trained in Chemistry at the University of Brasília (BSc – Bachelor, Teaching Degree, and Industrial Chemistry), I later completed my MSc in Catalysis before pursuing international doctoral training in France and collaborative research experiences in the Netherlands. Today, I serve as a Postdoctoral Researcher at the Federal Fluminense University (UFF) and as a Collaborating Researcher at the National Institute of Technology (INT), supported by Brazil’s National Council for Scientific and Technological Development (CNPq). With over a decade of experience in heterogeneous catalysis, I work on the design, preparation, and advanced characterization of supported catalytic materials and their application in biomass fractionation, esterification, dehydration, polymerization, photodegradation, and lignin depolymerization. Beyond publications and interdisciplinary projects, I am deeply engaged in mentoring students, fostering inclusive research environments, and promoting accessible, evidence-based scientific communication. I believe catalysis happens at multiple scales: in molecules, in ideas, and in people. By integrating fundamental science, data-driven approaches, and collaborative networks, my goal is to accelerate sustainable solutions while strengthening a resilient, cooperative scientific community.
    design:
      columns: '1'
      background:
        color:
          light: "#f9f9f9"
          dark: "#0f0f14"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
    
  # Filterable Portfolio - Alpine.js powered project filtering
  - block: portfolio
    id: projects
    content:
      title: "Featured Projects"
      subtitle: "A selection of my recent work"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: All
          tag: '*'
        - name: Full-Stack
          tag: Full-Stack
        - name: Frontend
          tag: Frontend
        - name: Backend
          tag: Backend
      default_button_index: 0
      # Archive link auto-shown if more projects exist than 'count' above
      # archive:
      #   enable: false  # Set to false to explicitly hide
      #   text: "Browse All"  # Customize text
      #   link: "/work/"  # Custom URL
    design:
      columns: 3
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Experience Timeline
  - block: resume-experience
    id: experience
    content:
      title: Experience
      date_format: Jan 2006
      items:
        - title: Senior Software Engineer
          company: Tech Corp
          company_url: ''
          company_logo: ''
          location: San Francisco, CA
          date_start: '2023-01-01'
          date_end: ''
          description: |-
            * Lead development of microservices architecture serving 1M+ users
            * Improved API response time by 40% through optimization
            * Mentored team of 5 junior developers
            * Tech stack: React, Node.js, PostgreSQL, AWS
        - title: Full-Stack Developer
          company: Startup Inc
          company_url: ''
          company_logo: ''
          location: Remote
          date_start: '2021-06-01'
          date_end: '2022-12-31'
          description: |-
            * Built and deployed 3 production applications from scratch
            * Implemented CI/CD pipeline reducing deployment time by 60%
            * Collaborated with design team on UI/UX improvements
            * Tech stack: Next.js, Express, MongoDB, Docker
        - title: Junior Developer
          company: Web Agency
          company_url: ''
          company_logo: ''
          location: New York, NY
          date_start: '2020-01-01'
          date_end: '2021-05-31'
          description: |-
            * Developed client websites using modern web technologies
            * Maintained and updated legacy codebases
            * Participated in code reviews and agile ceremonies
            * Tech stack: React, WordPress, PHP, MySQL
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Recent Blog Posts
  - block: collection
    id: blog
    content:
      title: Recent Posts
      subtitle: 'Thoughts on web development, tech, and more'
      text: ''
      filters:
        folders:
          - blog
        exclude_featured: false
      count: 3
      order: desc
    design:
      view: card
      columns: 3
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Contact Section
  - block: contact-info
    id: contact
    content:
      title: Get In Touch
      subtitle: "Let's build something amazing together"
      text: |-
        I'm always interested in hearing about new projects and opportunities.
        Whether you're looking to collaborate or just want to say hi, feel free to reach out!
      email: mateus_paiva@id.uff.br
      autolink: true
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        paddin
    g: ["4rem", "0", "4rem", "0"]
---




