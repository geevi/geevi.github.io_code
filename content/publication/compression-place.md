+++
title = "Compressing Models for Recognizing Places"
date = "2017-06-01"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Soham Saha", "Girish Varma", "CV Jawahar"]

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
publication = "In *Asian Conference on Pattern Recognision (ACPR'17)*."
publication_short = "In *ACPR*"

# Abstract and optional shortened version.
abstract = ""

# Featured image thumbnail (optional)
image_preview = ""

# Is this a selected publication? (true/false)
selected = true

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["model-compression"]

# Links (optional).
url_pdf =  "http://cvit.iiit.ac.in/images/ConferencePapers/2017/CompressingDeeNeural.pdf"
#url_preprint = "#"
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
Visual place recognition on low memory devices such as mobile phones and robotics systems is a challenging problem. The state of the art models for this task uses deep learning architectures having close to 100 million parameters which takes over 400MB of memory. This makes these models infeasible to be deployed in low memory devices and gives rise to the need of compressing them. Hence we study the effectiveness of model compression techniques like trained quantization and pruning for reducing the number of parameters on one of the best performing image retrieval models called NetVLAD. We show that a compressed network can be created by starting with a model pre-trained for the task of visual place recognition and then fine-tuning it via trained pruning and quantization. The compressed model is able to produce the same mAP as the original uncompressed network. We achieve almost 50% parameter pruning with no loss in mAP and 70% pruning with close to 2% mAP reduction, while also performing 8-bit quantization. Furthermore, together with 5-bit quantization, we perform about 50% parameter reduction by pruning and get only about 3% reduction in mAP.