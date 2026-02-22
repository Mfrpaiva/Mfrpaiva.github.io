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
          url: "#biography"
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
          <div style="width: 100vw; position: relative; left: 50%; right: 50%; margin-left: -50vw; margin-right: -50vw; padding: 2rem;">
            <div style="display: flex; align-items: flex-start; gap: 2rem; margin-bottom: 2rem; max-width: 1400px; margin: 0 auto; padding-right: 2rem;">
              <div style="flex: 0 0 35%; min-width: 250px;">
                <div style="margin-bottom: 2rem;">
                  <img src="/VFB.png" alt="Biography image" style="max-width: 100%; height: auto; border-radius: 8px; margin-bottom: 0.8rem;">
                  <p style="text-align: center; font-size: 0.85rem; color: #666; margin: 0;">Catalysts lower the energy barrier needed for the reaction to proceed.</p>
                </div>
                <div style="display: flex; flex-direction: column; align-items: center;">
                  <img src="/VFC.gif" alt="Biography image 2" style="max-width: 100%; height: auto; border-radius: 8px; margin-bottom: 0.8rem;">
                  <p style="text-align: center; font-size: 0.85rem; color: #666; margin: 0;">Science and its entire journey: Learning, Testing and Evolving.</p>
                </div>
              </div>
              <div style="flex: 1; text-align: justify; font-size: 1.10rem; line-height: 1.6;">
                <strong style="color: #4a9fd8;">"Catalyzing people and reactions"</strong> is more than a motto – it is the principle that has guided both my scientific journey and my way of engaging with others. In chemistry, catalysis accelerates transformations. In life, I strive to play a similar role: enabling progress, fostering collaboration, and empowering those around me to go further than they imagined possible. My academic path reflects this dual commitment to scientific advancement and collective growth. I hold a PhD in Materials Chemistry from the Université de Lille (France), awarded within the PEARL i-site / Marie Skłodowska-Curie Actions excellence framework and recognized with the European Doctorate Label. My doctoral research integrated catalysis and combustion toward advanced lignocellulosic biomass valorization, combining fundamental understanding with sustainable technological applications. Originally trained in Chemistry at the University of Brasília (BSc – Bachelor, Teaching Degree, and Industrial Chemistry), I later completed my MSc in Catalysis before pursuing international doctoral training in France and collaborative research experiences in the Netherlands. Today, I serve as a Postdoctoral Researcher at the Fluminense Federal University (UFF) and as a Collaborating Researcher at the National Institute of Technology (INT), supported by Brazil's National Council for Scientific and Technological Development (CNPq). With over a decade of experience in heterogeneous catalysis, I work on the design, preparation, and advanced characterization of supported catalytic materials and their application in different reactions, like biomass fractionation and hydrolysis, esterification, sugars dehydration, polymerization, photodegradation, and lignin depolymerization. Beyond publications and interdisciplinary projects, I am deeply engaged in mentoring students, fostering inclusive research environments, and promoting accessible, evidence-based scientific communication. I believe catalysis happens at multiple scales: in molecules, in ideas, and in people. By integrating fundamental science, data-driven approaches, and collaborative networks, my goal is to accelerate sustainable solutions while strengthening a resilient, cooperative scientific community.
                <br><br>
                🔎Research Interests: <strong style="color: #4a9fd8;">Heterogeneous catalysis | Biomass valorization | Sustainable materials | Circular processes | Data-driven approaches | Scientific mentoring</strong>
              <div style="margin-top: 2rem; text-align: center;">
                <a href="/uploads/Paiva_Mateus_CV.pdf" download style="display: inline-block; padding: 0.75rem 2rem; background-color: #4a9fd8; color: white; text-decoration: none; border-radius: 8px; font-weight: bold; transition: background-color 0.3s ease;">
                    📄 Download Resume
                  </a>
                </div>
              </div>
            </div>
          </div>
    design:
      background:
        color:
          light: "#f9f9f9"
          dark: "#0f0f14"
      spacing:
        padding: ["0", "0", "0", "0"]
        margin: ["0", "0", "0", "0"]
    
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
        padding: ["4rem", "0", "2rem", "0"]
  
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
        - name: Research
          tag: Full-Stack
        - name: Teaching
          tag: Frontend
        - name: Community Outreach
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
        padding: ["2rem", "0", "4rem", "0"]

    # Scientific Contributions
  - block: markdown
    id: scientificcontributions
    content:
      title: Scientific Contributions
      text: |
          <div style="width: 100vw; position: relative; left: 50%; right: 50%; margin-left: -50vw; margin-right: -50vw; padding: 2rem;">
            <div style="display: flex; align-items: flex-start; gap: 2rem; margin-bottom: 2rem; max-width: 1400px; margin: 0 auto; padding-right: 2rem;">
              <div style="flex: 0 0 55%; min-width: 250px;">
                <div style="margin-bottom: 2rem;">
                  <img src="/P2.png" alt="Biography image" style="max-width: 100%; height: auto; border-radius: 8px; margin-bottom: 0.8rem;">
                </div>
              </div>
              <div style="flex: 1; text-align: justify; font-size: 1.1rem; line-height: 1.6;">
                <strong style="color: #4a9fd8;"></strong><br><br>My research contributions span peer-reviewed publications in heterogeneous catalysis, inorganic chemistry, biomass valorization, and sustainable reaction engineering, alongside book chapters and numerous presentations at scientific meetings. I strongly believe that science advances through dialogue. Participation in national and international conferences is therefore not merely complementary, but fundamental to refining ideas, fostering collaborations, and contributing to the global chemistry community. A complete and updated list of publications and conference contributions is available for download below.
                <br><br>
                <div style="margin-top: 2rem; text-align: center;">
                  <a href="/uploads/Publications_MFP.pdf" download style="display: inline-block; padding: 0.75rem 2rem; background-color: #4a9fd8; color: white; text-decoration: none; border-radius: 8px; font-weight: bold; transition: background-color 0.3s ease;">
                    📄 Download Publication Record
                  </a>
              <div style="text-align: justify; font-size: 1.1rem; line-height: 1.6;">
                <strong style="color: #4a9fd8;"></strong><br><br>Beyond traditional outputs, my work is closely linked to extension and science communication initiatives. This includes outreach projects such as the award-winning video
                  <a href="https://youtu.be/psEIIGJiRBM?si=eYuQBZ_BH9v4Uu_M" target="_blank" rel="noopener noreferrer">
                    <span style="color: #4a9fd8;">“From a moment available, a useful force”</span>
                  </a> <strong style="color: #4a9fd8;"></strong> (Brazilian Catalysis Society – SBCat, 2020), as well as educational research on student retention and dropout in chemistry programs. Further details can be found in the <strong style="color: #4a9fd8;">Projects section</strong>.
            </div>
          </div>
    design:
      background:
        color:
          light: "#f9f9f9"
          dark: "#0f0f14"
      spacing:
        padding: ["0", "0", "0", "0"]
        margin: ["0", "0", "0", "0"]

# Distinctions Section
- block: markdown
  id: distinctions
  content:
    title: Awards & Distinctions
    text: |
      <div style="width: 100vw; position: relative; left: 50%; right: 50%; margin-left: -50vw; margin-right: -50vw; padding: 2rem;">
        <div style="display: flex; flex-direction: row; align-items: flex-start; gap: 2rem; max-width: 1400px; margin: 0 auto; padding-right: 2rem;">

          <!-- TEXT (LEFT) -->
          <div style="flex: 1; text-align: left; font-size: 1.05rem; line-height: 1.65;">
            <div style="margin-top: 0.25rem;">
              <div style="margin: 0 0 0.65rem 0;">🏆DivCat travel fellowship – Support to attend the 18th International congress on catalysis (ICC), French chemical society (SCF), France (2024)</div>
              <div style="margin: 0 0 0.65rem 0;">🏆Group Award – Best Technological Invention, Unite! Biomass Winter School (U! Bio), International School of Paper, Print Media and Biomaterials (INP-PAGORA), France (2023)</div>
              <div style="margin: 0 0 0.65rem 0;">🏆Group Award - Best Start-up Project Management, Innovation Challenge - Université de Lille (UNIV-LILLE), France (2023)</div>
              <div style="margin: 0 0 0.65rem 0;">🏆Éole excellence fellowship – academic research stay in the Netherlands, Franco–Dutch higher education and research network (RFN), France (2021)</div>
              <div style="margin: 0 0 0.65rem 0;">🏆Dmitri Mendeleev award – Outstanding student award, Regional council of chemistry (CRQ-XII), Brazil (2021)</div>
              <div style="margin: 0 0 0.65rem 0;">🏆Best poster awards (Physical Chemistry and Catalysis Divisions) – 38th RA, 42nd RA and IV ERCO Meetings, Brazilian Chemical Society (SBQ), Brazil (2015, 2019 and 2021)</div>
              <div style="margin: 0 0 0.65rem 0;">🏆ICC Young scientists travel award – International Association of Catalysis Societies (IACS), United States (2020)</div>
              <div style="margin: 0 0 0.65rem 0;">🏆Outstanding scientific video award for research communication (Master’s level) – Brazilian Catalysis Society (SBCat), Brazil, (2020)</div>
              <div style="margin: 0 0 0.65rem 0;">🏆Honorable Mention - Outstanding Student, Centro Interescolar de Línguas de Brasília (CIL) (2016 and 2017).</div>
              <div style="margin: 0;">🏆Honorable mentions in exact sciences – Undergraduate research congresses, University of Brasília (UnB) (2015 and 2016).</div>
            </div>
          </div>

          <!-- IMAGE (RIGHT) -->
          <div style="flex: 0 0 32%; min-width: 240px;">
            <img src="/Prize.png" alt="Awards and distinctions" style="max-width: 100%; height: auto; border-radius: 10px;">
          </div>

        </div>
      </div>
  design:
    background:
      color:
        light: "#f9f9f9"
        dark: "#0f0f14"
    spacing:
      padding: ["0", "0", "0", "0"]
      margin: ["0", "0", "0", "0"]
    
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
        padding: ["2rem", "0", "0rem", "0"]

    # Final Phrase
  - block: markdown
    id: 
    content:
      title: 
      subtitle: 
      text: |-
        <p align="center">
          <em>
          “There are countless definitions of purpose, but the most meaningful one, to me, is when we think about the sunflower. Everyone knows that it turns toward the Sun. What not everyone knows is that, when there is little sunlight, sunflowers turn toward one another to share light. Purpose is exactly that: directing our potential in order to impact other people and the world.” — Arnaldo Neto
          <em>
        </p>
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["0rem", "0", "4rem", "0"]
---




