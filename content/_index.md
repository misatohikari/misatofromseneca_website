---
# Leave the homepage title empty to use the site title
title: ''
date: 2024-05-14
type: landing

sections:
  - block: about.biography
    id: about
    # demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: About Me
      username: admin
  - block: features
    content:
      title: Skills
      items:
        - name: Software Testing & QA
          description: Functional, regression, integration & E2E
          icon: vial
          icon_pack: fas
        - name: Python
          description:
          icon: python
          icon_pack: fab
        - name: SQL & Databases
          description:
          icon: database
          icon_pack: fas
        - name: Java
          description:
          icon: java
          icon_pack: fab
        - name: AWS Cloud
          description:
          icon: aws
          icon_pack: fab
        - name: Git
          description:
          icon: git-alt
          icon_pack: fab
  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Cloud Support Associate
          company: Amazon Web Services
          company_url: 'https://aws.amazon.com/'
          company_logo:
          location: Toronto, Canada
          date_start: '2026-04-01'
          date_end: ''
          description: |2-
              - Triage and resolve high-severity networking cases (VPC, ALB, TLS, API connectivity) for global enterprise clients under tight SLOs, minimizing revenue-impacting downtime for production traffic.
              - Trace failures across interconnected AWS services (IAM, security groups, route tables, DNS, load balancers) using first-principles analysis to identify root causes that surface-level diagnosis would miss.
              - Analyze customer and AWS-side network logs (CloudWatch, CloudTrail, VPC Flow Logs) to separate customer configuration issues from platform-level defects.
              - Document reproduction steps and root cause findings for AWS engineering teams, including service-side defects, leading to confirmed fixes that prevented recurrence for other customers.
        - title: IT QA Assistant (Co-op)
          company: Ministry of Education, Government of Ontario
          company_url: ''
          company_logo:
          location: Toronto, Canada
          date_start: '2024-09-01'
          date_end: '2025-04-30'
          description: |2-
              - Executed 200+ test cases across functional, regression, smoke, integration, and E2E testing for Ontario's OSAP student financial aid platform (400,000+ students per academic year), covering the student portal, admin portal, and institutional views.
              - Identified and triaged 50+ defects in HP ALM with severity classification and reproduction steps; performed confirmation and regression testing after fixes, and maintained traceability matrices to support UAT and release sign-off.
              - Served as the primary co-op QA resource for the Ontario Learn and Stay Grant module, testing complex eligibility scenarios (student withdrawal, employment registration, six-month compliance deadlines) alongside the BA lead.
              - Developed net-new test cases from business requirements and Figma design flows, and validated cross-portal data consistency between student-facing behavior and admin-side updates.
        - title: Digital Marketing Intern
          company: Life Journey Global
          company_url: ''
          company_logo:
          location: Toronto, Canada
          date_start: '2022-02-01'
          date_end: '2022-05-31'
          description: Developed and maintained company websites using WordPress, HTML, and CSS to deliver user-friendly interfaces, and implemented SEO strategies that improved search engine rankings and organic traffic.
      design:
      columns: '2'
  - block: markdown
    id: certifications
    content:
      title: Certifications
      text: |-
        - **[AWS Certified Solutions Architect – Associate](https://www.credly.com/badges/c50b6d6e-ed43-4bb4-b4f1-a521ff00a756/linked_in_profile)** — Amazon Web Services (2026)
        - **[AWS Certified Cloud Practitioner](https://www.credly.com/badges/56ace733-db2e-44d8-b574-af20da1fa499/linked_in_profile)** — Amazon Web Services (2025)
        - **[Selenium Essential Training](https://www.linkedin.com/in/misato-yoshimoto/details/certifications/)** — LinkedIn Learning (2024)
        - **ISTQB Certified Tester, Foundation Level (CTFL v4.0)** — In progress
    design:
      columns: '1'
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
        - name: C++
          tag: CPP
        - name: Web Development
          tag: Web Development
      design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
        columns: '2'
        view: showcase
        # For Showcase view, flip alternate rows?
        flip_alt_rows: false
  # - block: accomplishments
  #   content:
  #     # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
  #     title: 'Accomplish&shy;ments'
  #     subtitle:
  #     # Date format: https://docs.hugoblox.com/customization/#date-format
  #     date_format: Jan 2006
  #     # Accomplishments.
  #     #   Add/remove as many `item` blocks below as you like.
  #     #   `title`, `organization`, and `date_start` are the required parameters.
  #     #   Leave other parameters empty if not required.
  #     #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #     items:
  #       - certificate_url: https://www.coursera.org
  #         date_end: ''
  #         date_start: '2021-01-25'
  #         description: ''
  #         icon: coursera
  #         organization: Coursera
  #         organization_url: https://www.coursera.org
  #         title: Neural Networks and Deep Learning
  #         url: ''
  #       - certificate_url: https://www.edx.org
  #         date_end: ''
  #         date_start: '2021-01-01'
  #         description: Formulated informed blockchain models, hypotheses, and use cases.
  #         icon: edx
  #         organization: edX
  #         organization_url: https://www.edx.org
  #         title: Blockchain Fundamentals
  #         url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
  #       - certificate_url: https://www.datacamp.com
  #         date_end: '2020-12-21'
  #         date_start: '2020-07-01'
  #         description: ''
  #         icon: datacamp
  #         organization: DataCamp
  #         organization_url: https://www.datacamp.com
  #         title: 'Object-Oriented Programming in R'
  #         url: ''
  #   design:
  #     columns: '2'
  # - block: collection
  #   id: posts
  #   content:
  #     title: Recent Posts
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
  #     title: Recent Publications
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
  #     # Choose a map provider in `params.yaml` to show a map from these coordinates
  #     coordinates:
  #       latitude: '37.4275'
  #       longitude: '-122.1697'  
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
