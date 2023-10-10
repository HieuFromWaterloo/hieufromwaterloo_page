---
# Leave the homepage title empty to use the site title
title:
date: 2023-10-09
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About Me
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: features
    content:
      title: Skills
      items:
        - name: Machine/Deep Learning
          description:
          icon: robot
          icon_pack: fas
        - name: Python
          description: 
          icon: python
          icon_pack: fab
        - name: Database (SQL/noSQL)
          description: 
          icon: database
          icon_pack: fas
        - name: AWS
          description: 
          icon: aws
          icon_pack: fab
        - name: Github
          description: 
          icon: github
          icon_pack: fab
        - name: Docker
          description:
          icon: docker
          icon_pack: fab
  - block: experience
    id: experiences
    content:
      title: Experiences
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Tech Co-founder
          company: b(x) Theory Inc.
          company_url: 'https://bxtheory.com/'
          company_logo:
          location: Toronto, Canada
          date_start: '2023-07-01'
          date_end: '2023-08-01'
          description: Developed analytic solutions for financial and operational restructuring opportunities
        - title: Data Scientist
          company: Godaddy Inc.
          company_url: 'https://www.godaddy.com/'
          company_logo:
          location: Santa Clara, United States (Remote)
          date_start: '2021-05-01'
          date_end: '2022-07-01'
          description: Collaborated within a high-performing data science team that develops deep learning models for GoDaddy’s core global domain business
        - title: Data Scientist
          company: Royal Bank of Canada - DNA Group
          company_url: 'https://www.rbcroyalbank.com/'
          company_logo:
          location: Toronto, Canada (Remote)
          date_start: '2020-01-05'
          date_end: '2022-05-01'
          description: Collaborated with RBC's Canadian Banking Operations to develop and deploy NLP solutions, which was designed to improve current business process \& saved expenses per year.
        - title: Various Internships in Data Science and Software Engineering
          company: RBC Capital Markets, RBC Global Cybersecurity, and Marsh Canada Ltd
          company_url: 'https://www.rbcroyalbank.com/'
          company_logo:
          location: Toronto, Canada
          date_start: '2017-05-01'
          date_end: '2019-09-01'
          description:
    design:
      columns: '2'
  - block: accomplishments
    id: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Certificates'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.coursera.org/account/accomplishments/specialization/5AJPZYV3EFG5
          date_end: ''
          date_start: '2019-12-31'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Deep Learning Specialization - DeepLearning.AI
          url: https://www.coursera.org/account/accomplishments/specialization/5AJPZYV3EFG5
        - certificate_url: uploads/certs/cousera_advanced_ml.pdf
          date_end: ''
          date_start: '2020-05-01'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Advanced Machine Learning Specialization - HSE University
          url: uploads/certs/cousera_advanced_ml.pdf
        - certificate_url: https://www.coursera.org/account/accomplishments/specialization/certificate/AL529YFFENYJ
          date_end: ''
          date_start: '2020-09-01'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Data Science Foundations using R - Johns Hopkins University
          url: https://www.coursera.org/account/accomplishments/specialization/certificate/AL529YFFENYJ
        - certificate_url: https://www.coursera.org/account/accomplishments/specialization/YYFTLH83ETCZ
          date_end: ''
          date_start: '2021-01-31'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Software Design and Architecture - University of Alberta
          url: https://www.coursera.org/account/accomplishments/specialization/YYFTLH83ETCZ
    design:
      columns: '2'
  # - block: collection
  #   id: posts
  #   content:
  #     title: Posts
  #     subtitle: ''
  #     text: ''
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       folders:
  #         - post
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: compact
  #     columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Machine Learning
          tag: Machine Learning
        - name: Stat/Math
          tag: StatMath
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  # - block: markdown
  #   content:
  #     title: Gallery
  #     subtitle: ''
  #     text: |-
  #       {{< gallery album="demo" >}}
  #   design:
  #     columns: '1'
  # - block: collection
  #   id: featured
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     columns: '2'
  #     view: card
  # - block: collection
  #   content:
  #     title: Publications
  #     text: |-
  #       {{% callout note %}}
  #       Quickly discover relevant content by [filtering publications](./publication/).
  #       {{% /callout %}}
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: true
  #   design:
  #     columns: '2'
  #     view: citation
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     columns: '2'
  #     view: compact
  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
  # - block: contact
  #   id: contact
  #   content:
  #     title: Contact
  #     subtitle:
  #     text: |-
  #       Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
  #     # Contact (add or remove contact options as necessary)
  #     email: test@example.org
  #     phone: 888 888 88 88
  #     appointment_url: 'https://calendly.com'
  #     address:
  #       street: 450 Serra Mall
  #       city: Stanford
  #       region: CA
  #       postcode: '94305'
  #       country: United States
  #       country_code: US
  #     directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
  #     office_hours:
  #       - 'Monday 10:00 to 13:00'
  #       - 'Wednesday 09:00 to 10:00'
  #     contact_links:
  #       - icon: twitter
  #         icon_pack: fab
  #         name: DM Me
  #         link: 'https://twitter.com/Twitter'
  #       - icon: skype
  #         icon_pack: fab
  #         name: Skype Me
  #         link: 'skype:echo123?call'
  #       - icon: video
  #         icon_pack: fas
  #         name: Zoom Me
  #         link: 'https://zoom.com'
  #     # Automatically link email and phone or display as text?
  #     autolink: true
  #     # Email form provider
  #     form:
  #       provider: netlify
  #       formspree:
  #         id:
  #       netlify:
  #         # Enable CAPTCHA challenge to reduce spam?
  #         captcha: false
  #   design:
  #     columns: '2'
---
