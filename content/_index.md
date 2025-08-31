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
      title: Core Technologies & Skills
      items:
        - name: Machine/Deep Learning
          description: NLP/LLM, search/ranking, and distributed ML systems with focus on business impact
          icon: robot
          icon_pack: fas
        - name: Programming & Data
          description: Python, SQL for scalable data processing and analysis with statistical and mathematical foundations
          icon: python
          icon_pack: fab
        - name: Infrastructure & Cloud
          description: AWS, Databricks, Docker, Kubernetes, Terraform for high-performance ML system deployment
          icon: cloud
          icon_pack: fas
        - name: Data Engineering
          description: Spark, Apache Airflow, dbt, Redis, MongoDB for robust data pipelines and distributed systems
          icon: database
          icon_pack: fas
        - name: MLOps & Automation
          description: GitHub Actions, CI/CD pipelines, model versioning and monitoring for scalable ML operations
          icon: github
          icon_pack: fab
        - name: Web Frameworks
          description: Flask, Django for building production ML services and APIs with high availability
          icon: code
          icon_pack: fas
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
        - title: "Senior Data Scientist"
          company: "Indeed - Trust & Safety Science"
          company_url: https://indeed.com
          company_logo:
          location: Toronto, Canada
          date_start: '2025-03-01'
          date_end: ''
          description: |2-
            • We help people get jobs while keeping our users and platform safe
        - title: Machine Learning Engineer/Data Scientist
          company: "McAfee - Browser Security Product"
          company_url: https://mcafee.com
          company_logo:
          location: Toronto, Canada
          date_start: '2024-03-01'
          date_end: '2025-03-01'
          description: |2-
            • Led end-to-end MLOps Strategy & Cloud Architecture for McAfee's Search Acceleration initiative (half billion dollar business)

            • Designed and deployed high-performance ML infrastructure using Terraform, Databricks Assets Bundle (IaC) and GitHub Actions, reducing model deployment time by over 50%

            • Led ML service design and deployment on AWS supporting 200M+ weekly active devices with 99.99% availability worldwide and 95th percentile response time under 100ms
        - title: Technical Co-Founder
          company: "b(x) Theory - Insolvency Analytics"
          company_url:
          company_logo:
          location: Toronto, Canada
          date_start: '2022-08-01'
          date_end: '2023-09-01'
          description: |2-
            • Along with the team, did whatever necessary to actualize b(x) Theory, an innovative fintech service that leverages high quality data, intuitive visualization and machine learning to transform how financial advisors, c-suite executives manage risks and identify opportunities in restructuring/special situations in Canada.

        - title: NLP Data Scientist
          company: "GoDaddy - Domain Search/Ranking"
          company_url: https://godaddy.com
          company_logo:
          location: Toronto, Canada
          date_start: '2021-04-01'
          date_end: '2022-08-01'
          description: |2-
            • Led end-to-end research, development, and deployment of novel NLP deep learning services on AWS (ECS, EC2, EMR, SageMaker)

            • Achieved under 20ms inference latency per request with 99.99% service availability across global markets for domain name auto-completion

            • Delivered 18% uplift in premium domain sales, 16% surge in search volumes, and 30% increase in click-through rates, resulting in $20M+ USD annual SERP revenue increase

            • Enhanced performance through personalization based on language, region, and device preferences using FNet, Transformers, BERT, CNN, and bi-directional LSTM architectures
        - title: NLP Data Scientist
          company: "Royal Bank of Canada - Email & Payment Analytics"
          company_url: https://rbc.com
          company_logo:
          location: Toronto, Canada
          date_start: '2020-01-01'
          date_end: '2021-04-01'
          description: |2-
            • Led R&D of NLP solution for Canadian Banking Operations to detect crucial payment-related emails from commercial clients nationwide

            • Transformed unsupervised text classification into semi-supervised learning paradigm, boosting true positive rates by 19% while reducing false negatives by 35%

            • Achieved projected annual savings of $1M CAD through advanced techniques including topic modeling with LDA, XGBoost and BERT embeddings
        - title: Various Internships in Data Science and Software Engineering
          company: RBC Capital Markets, RBC Global Cybersecurity, and Marsh Canada Ltd
          company_url:
          company_logo:
          location: Toronto, Canada
          date_start: '2017-05-01'
          date_end: '2019-09-01'
          description: Gained foundational experience in data science, software engineering, and financial technology across multiple industry-leading organizations.
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
          title: Deep Learning Specialization - DeepLearning.ai
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
        - certificate_url: https://www.coursera.org/account/accomplishments/certificate/WFME2P9Z27MM
          date_end: ''
          date_start: '2023-11-30'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Generative AI with Large Language Models - DeepLearning.ai
          url: https://www.coursera.org/account/accomplishments/certificate/WFME2P9Z27MM
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Personal Blog
      subtitle: 'Notes on ML/AI'
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: research
    content:
      title: Research/Projects
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
        - name: ML Engineer
          tag: ML Engineer
        - name: Data Engineer
          tag: Data Engineer
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
