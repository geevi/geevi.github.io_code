+++
title = "Class2Str: End to End Latent Hierarchy Learning"
date = "2018-03-01"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Soham Saha", "Girish Varma", '''<a href="https://faculty.iiit.ac.in/~jawahar/">C V Jawahar</a>''']

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference proceedings
# 2 = Journal
# 3 = Work in progress
# 4 = Technical report
# 5 = Book
# 6 = Book chapter
publication_types = ["1"]

# Publication name and optional abbreviated version.
publication = "International Conference on Pattern Recognision (<strong>ICPR</strong>)"
#publication_short = "In *ACPR*"

# Abstract and optional shortened version.
abstract = ""

bibtex='''
@InProceedings{SVJ18,
author = {Saha, Soham and Varma, Girish and Jawahar, C.V.},
title = {Class2Str: End to End Latent Hierarchy Learning},
booktitle = {International Conference on Pattern Recognision (ICPR)}.
year = {2018}
}
'''

# Featured image thumbnail (optional)
image_preview = "/img/cls2str.png"

# Is this a selected publication? (true/false)
selected = false

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["model-compression", "latent heirarchy"]

# Links (optional).
url_pdf = "" 
url_preprint = "https://arxiv.org/abs/1808.06675"
url_code = "https://github.com/Soham0/Class2Str"
#url_dataset = "#"
#url_project = "#"
#url_slides = "#"
#url_video = "#"
url_poster = "/pdfs/ICPR_2018_Poster.pdf"
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
Deep neural networks for image classification typically consists of a convolutional feature extractor followed by a fully connected classifier network. The predicted and the ground truth labels are represented as one hot vectors. Such a representation assumes that all classes are equally dissimilar. However, classes have visual similarities and often form a hierarchy. Learning this latent hierarchy explicitly in the architecture could provide invaluable insights. We propose an alternate architecture to the classifier network called the Latent Hierarchy (LH) Classifier and an end to end learned Class2Str mapping which discovers a latent hierarchy of the classes. We show that for some of the best performing architectures on CIFAR and Imagenet datasets, the proposed replacement and training by LH classifier recovers the accuracy, with a fraction of the number of parameters in the classifier part. Compared to the previous work of HDCNN, which also learns a 2 level hierarchy, we are able to learn a hierarchy at an arbitrary number of levels as well as obtain an accuracy improvement on the Imagenet classification task over them. We also verify that many visually similar classes are grouped together, under the learnt hierarchy.