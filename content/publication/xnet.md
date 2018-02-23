+++
title = "Deep Expander Networks: Efficient Deep Networks from Graph Theory"
date = "2017-11-15"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Ameya Prabhu", "Girish Varma", "Anoop Namboodiri"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference proceedings
# 2 = Journal
# 3 = Work in progress
# 4 = Technical report
# 5 = Book
# 6 = Book chapter
publication_types = ["4"]

# Publication name and optional abbreviated version.
publication = "arXiv"
#publication_short = "In *ACPR*"

# Abstract and optional shortened version.
abstract = ""

# Featured image thumbnail (optional)
image_preview = ""

# Is this a selected publication? (true/false)
selected = true

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["model-compression", "xnet"]

# Links (optional).
url_pdf = "https://arxiv.org/abs/1711.08757" 
url_preprint = "https://arxiv.org/abs/1711.08757"
#url_code = "#"
#url_dataset = "#"
#url_project = "#"
#url_slides = "#"
#url_video = "#"
#url_poster = "#"
#url_source = "#"

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
#url_custom = [{name = "Custom Link", url = "http://example.org"}]

# Does the content use math formatting?
#math = true

# Does the content use source code highlighting?
#highlight = true

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
#image = "headers/bubbles-wide.jpg"
#caption = "My caption :smile:"

+++
Deep Neural Networks, while being unreasonably effective for several vision tasks, have their usage limited by the computational and memory requirements, both during training and inference stages. Analyzing and improving the connectivity patterns between layers of a network has resulted in several compact architectures like GoogleNet, ResNet and DenseNet-BC. In this work, we utilize results from graph theory to develop an efficient connection pattern between consecutive layers. Specifically, we use {\it expander graphs} that have excellent connectivity properties to develop a sparse network architecture, the deep expander network (X-Net). The X-Nets are shown to have high connectivity for a given level of sparsity. We also develop highly efficient training and inference algorithms for such networks. Experimental results show that we can achieve the similar or better accuracy as DenseNet-BC with two-thirds the number of parameters and FLOPs on several image classification benchmarks. We hope that this work motivates other approaches to utilize results from graph theory to develop efficient network architectures. 