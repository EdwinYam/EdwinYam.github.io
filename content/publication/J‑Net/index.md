---
title: 'J‑Net: Randomly Weighted U‑Net for Audio Source Separation'
authors:
  - admin
  - Yen‑Min Hsu
  - Hung‑Yi Lee

commentable: true
date: '2019-11-29T00:00:00Z'
doi: '10.48550/arXiv.1911.12926'

# Schedule page publish date (NOT publication's date).
publishDate: '2019-11-29T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "ArXiv preprint"
publication_short: ""

abstract: "<p style='text-align: justify;'>Several results in the computer vision literature have shown the potential of randomly weighted neural networks. While they perform fairly well as feature extractors for discriminative tasks, there is a positive correlation between their performance and their fully trained counterparts. Based on these discoveries, we pose two questions: What is the value of randomly weighted networks in difficult generative audio tasks such as audio source separation? And does such a positive correlation still exist when it comes to large random networks and their trained counterparts?

In this paper, we demonstrate that the positive correlation indeed still exists. Building on this discovery, we can explore different architecture designs or techniques without training the entire model. Moreover, we found a surprising result that, compared to the non-trained encoder (down-sample path) in Wave-U-Net, fixing the decoder (up-sample path) to random weights results in better performance, almost comparable to the fully trained model."

# Summary. An optional shortened abstract.
summary: Randomly weighted neural networks have potential in computer vision and demonstrate a positive correlation in performance with fully trained models. This paper confirms the continued positive correlation and explores the value of randomly weighted networks in audio source separation, a challenging generative audio task.

tags:
  - Neural Architecture Search
  - Audio Source Separation
  - Digital Speech Processing

featured: true

links:
#- name: Custom Link
#  url: http://example.org
url_pdf: 'https://arxiv.org/pdf/1911.12926.pdf'
url_code: 'https://github.com/EdwinYam/J-Net'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Architecture of J-Net'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
