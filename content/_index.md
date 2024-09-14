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
        - name: JavaScript
          description:
          icon: js
          icon_pack: fab
        - name: Python
          description: 
          icon: python
          icon_pack: fab
        - name: C++
          description:
          icon: c
          icon_pack: fas
        - name: Node.js
          description: 
          icon: node
          icon_pack: fab
        - name: Database (SQL/noSQL)
          description: 
          icon: database
          icon_pack: fas
        - name: Github
          description: 
          icon: github
          icon_pack: fab
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
        - title: Software QA Engineer
          company: Ministry of Education
          company_url: ''
          company_logo: 
          location: Toronto, Canada
          date_start: '2024-09-04'
          date_end: ''
          description: I perform both manual and automated testing on the OSAP (Ontario Student Assistance Program) application using various tools. I also create logs of the test results and work closely with developers to contribute to bug fixes and feature improvements.
        - title: Restaurant Server
          company: Ikkousha Ramen
          company_url: ''
          company_logo: 
          location: Toronto, Canada
          date_start: '2021-05-01'
          date_end: ''
          description: I utilize my strong multitasking and proactive customer service skills to ensure a seamless dining experience for our guests. Additionally, I leverage my experience in team training to support fellow staff members, fostering a collaborative environment focused on delivering exceptional service.
        - title: Digital Marketing Internship
          company: Life Journey Global
          company_url: ''
          company_logo: 
          location: Toronto, Canada
          date_start: '2022-02-01'
          date_end: '2022-05-31'
          description: In my time at the position, I was responsible for the development and maintenance of company websites using WordPress. By incorporating HTML and CSS, I ensured user-friendly interfaces and seamless functionality. Additionally, I implemented Search Engine Optimization (SEO) strategies, resulting in a notable 20% increase in search engine rankings and organic traffic.
        - title: Telephone Inquiry & Sales Representative
          company: Bellclick
          company_url: ''
          company_logo: 
          location: Osaka, Japan
          date_start: '2020-03-01'
          date_end: '2020-10-31'
          description: Throughout my role, I actively provided exceptional customer support by promptly addressing inquiries, swiftly troubleshooting issues, and professionally resolving concerns. As a testament to my dedication, I received recognition for my outstanding performance, earning awards for consistently achieving high customer satisfaction scores of over 4.6 out of 5. Moreover, I showcased my strong sales acumen by consistently meeting or surpassing personal sales targets of 140 sales per month.
        - title: Salesclerk
          company: Tsuruha Drug
          company_url: ''
          company_logo: 
          location: Osaka, Japan
          date_start: '2018-11-01'
          date_end: '2020-10-31'
          description: During my time, I played a pivotal role in assisting customers by providing personalized product recommendations tailored to their specific needs, always delivered with a focus on providing supportive service. Through these efforts, I successfully achieved monthly sales targets. Additionally, I took on the responsibility of training new customer service hires, imparting essential skills and knowledge to promote efficiency and professionalism within the team.
      design:
      columns: '2'
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
