---
title: Determining clinically relevant features in cytometry data using persistent homology
summary: TDA helps to identify structural difference in single-cell cytometry data.
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
url_code: "https://github.com/soham0209/Biosketch"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

Cytometry experiments yield high-dimensional point cloud data that is difficult to interpret manually. Boolean gating techniques coupled with comparisons of relative abundances of cellular subsets is the current standard for cytometry data analysis. However, this approach is unable to capture more subtle topological features of data, especially if those features are masked by data transforms. We propose that persistent homology, a mathematical technique for summarizing the topology of a dataset, will be capable of uncovering systematic topological differences between differing sources of data. Publicly available cytometry data describing non-naïve CD8+ T-cells in COVID-19 patients and healthy controls motivates our method, and we show that systematic structural differences exist between protein expressions in COVID-19 patients and healthy controls.

Our method identifies proteins of interest given their importance to an XGBoost classifier to pass to a kernel-density estimator (KDE). We then compute persistence diagrams on points sampled from the KDEs. The resulting persistence diagrams identify regions in cytometry datasets of differing density with the $H_0$ barcodes, and identify geometric structures composed of loops, which are representative of length scales in the data, with the $H_1$ barcodes. We calculated Wasserstein distances between these persistence diagrams for random pairs of healthy controls and COVID-19 patients and found that systematic structural differences exist between COVID-19 patients and healthy controls in the expression data for T-bet, Eomes, and Ki-67. Further analysis shows that expression of T-bet and Eomes are significantly downregulated in COVID-19 patient non-naïve CD8+ T-cells compared to healthy controls. This counter-intuitive finding might indicate that Effector CD8+ T-cells are less prevalent in COVID-19 patients than healthy controls. This method is applicable to any cytometry dataset to discover novel topological insights that would be difficult to ascertain with a standard gating strategy or with large batch effects in the data.
