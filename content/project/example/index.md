---
title: Predicting phenotypes using topology and machine learning
summary: TDA helps to identify phenotypes.
tags:
- Deep Learning
- TDA
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
# - icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: "https://github.com/soham0209/Gene-Expression"
url_pdf: ""
url_slides: ""
url_video: "https://drive.google.com/file/d/1tbZ7d6uDurdl4OgnbqTSyXtOTWc_f2rc/view?usp=sharing"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

## Background

Interpretation of high-throughput gene expression data continues to require mathematical tools in data analysis that recognizes the shape of the data in high dimensions. Topological data analysis(TDA) has recently been successful in extracting robust features in several applications dealing with high dimensional constructs. In this work, we utilize some recent developments in TDA to curate gene expression data. Our work differs from the predecessors in two aspects: (1) Traditional TDA pipelines use topological signatures called barcodes to enhance feature vectors which are used for classification. In contrast, this work involves curating relevant features to obtain somewhat better representatives with the help of TDA. This representatives of the entire data facilitates better comprehension of the phenotype labels. (2) Most of the earlier works employ barcodes obtained using topological summaries as fingerprints for the data. Even though they are stable signatures, there exists no direct mapping between the data and said barcodes.
## Results
The topology relevant curated data that we obtain provides an improvement in shallow learning as well as deep learning based supervised classifications. We further show that the representative cycles we compute have an unsupervised inclination towards phenotype labels. This work thus shows that topological signatures are able to comprehend gene expression levels and classify cohorts accordingly.
## Conclusions
In this work, we engender representative persistent cycles to discern the gene expression data. These cycles allow us to directly procure genes entailed in similar processes.
