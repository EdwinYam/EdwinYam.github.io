---
# Leave the homepage title empty to use the site title
title: 陳柏文
date: 2023-06-21
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin

  - block: features
    id: skills
    content:
      title: Skills
      items:
        - name: Python
          description: Fairseq, Pytorch, Tensorflow 
          icon: python
          icon_pack: fab
        - name: C/C++
          description: Kaldi
          icon: c
          icon_pack: fass
        - name: Digit Speech Processing
          description: Text-to-Speech, Automatic Speech Recognition
          icon: microphone-alt
          icon_pack: fas

  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Graduate Researcher
          company: Speech Processing & Machine Learning Laboratory, NTU
          company_url: 'https://speech.ee.ntu.edu.tw/~hylee/index.php'
          company_logo: ""
          location: Taipei, Taiwan
          date_start: '2018-09-01'
          date_end: '2022-11-10'
          description: |2-
            Advisor: Prof. Hung-Yi Lee

            * Conducted research in speech processing and acoustic modeling utilizing deep learning techniques to explore novel topics
            * Proposed the first duplex speech chain model capable of performing Text‑to‑Speech and Automatic Speech Recognition simultaneously through the use of a single reversible network, enabling the effective use of supervision signals from both directions
            * Proposed a rapid neural architecture search approach on audio source separation that utilizes the positive correlation in performance shown between models with fixed rando mly weighted layers and their fully trained counterparts 
            * Served as a reviewer for ICASSP 2020
        - title: Software Engineer Intern
          company: Acoustic and Speech Processing Team of Multimedia Department, MediaTek
          company_url: 'https://www.mediatek.com/'
          company_logo: ""
          location: Hsinchu, Taiwan
          date_start: '2017-07-01'
          date_end: '2017-08-31'
          description: |2-
            * Compressed acoustic models via knowledge distillation, maintaining a modest performance decline with 50% fewer parameters
            * Created a toolkit to facilitate seamless migration of acoustic models from Kaldi to Tensorflow, effectively reducing development time
        - title: Research Intern
          company: Institute of Information Science, Academia Sinica
          company_url: 'https://www.iis.sinica.edu.tw/en/index.html'
          company_logo: ""
          location: Taipei, Taiwan
          date_start: '2016-07-01'
          date_end: '2016-08-31'
          description: |2-
            * Reimplemented a super‑resolution model, which predicted the residual between the original image and its super‑resolved counterpart
    design:
      columns: '2'
  
  - block: collection
    id: publications 
    content:
      title: Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation

  - block: accomplishments
    id: awards
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Awards'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: ''
          date_end: ''
          date_start: '2020-04-01'
          description: |2-
            * Achieved 8th place out of 469 teams on the leaderboard as team leader
            * Used pretrained language models, SCIBERT, with additional linear layers to perform sequential sentence classification
          organization: Ministry of Education, Taiwan
          organization_url: https://tbrain.trendmicro.com.tw/Competitions/Details/8
          title: Honorable Mention Award
          url: 'https://github.com/EdwinYam/AICUP2019-Abstract_Labeling'
    design:
      columns: '2'
  
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
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false

  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
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

  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'

  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle: ''
      text: ''
      # Contact (add or remove contact options as necessary)
      email: edwinyam@proton.me
      appointment_url: 'https://calendly.com'
      address:
        street: ''
        city: Taipei
        region: ''
        postcode: ''
        country: Taiwan
        country_code: TW

      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
