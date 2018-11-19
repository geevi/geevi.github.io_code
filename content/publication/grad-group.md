+++
title = "Efficient Semantic Segmentation using Gradual Grouping"
date = "2018-05-01"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Nikitha Vallurupalli", "Sriharsha Annamaneni", "Girish Varma", '''<a href="https://faculty.iiit.ac.in/~jawahar/">C V Jawahar</a>''', "Manu Mathew", "Soyeb Nagori"]

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
publication = '''<span style='color: orange'>Best Runner-Up Award, Oral Presentation</span><br/><a href='https://embeddedvisionworkshop.wordpress.com/'>IEEE Embedded Vision Workshop, CVPR'18</a>'''
#publication_short = "In *ACPR*"

# Abstract and optional shortened version.
abstract = ""

# Featured image thumbnail (optional)
image_preview = "/img/grad.png"

# Is this a selected publication? (true/false)
selected = false

bibtex='''
@InProceedings{Vallurupalli_2018_CVPR_Workshops,
author = {Vallurupalli, Nikitha and Annamaneni, Sriharsha and Varma, Girish and Jawahar, C.V. and Mathew, Manu and Nagori, Soyeb},
title = {Efficient Semantic Segmentation Using Gradual Grouping},
booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
month = {June},
year = {2018}
}
'''

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["model-compression", "auto-nav"]

# Links (optional).
url_pdf = "http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w12/Vallurupalli_Efficient_Semantic_Segmentation_CVPR_2018_paper.pdf" 
#url_preprint = "https://arxiv.org/abs/1711.08757"
#url_code = "#"
#url_dataset = "#"
#url_project = "#"
url_slides = "/pdfs/cvpr-evw-18-slides.pdf"
#url_video = "#"
url_poster = "/pdfs/cvpr-evw-18-poster.pdf"
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
Deep CNNs for semantic segmentation have high memory and run time requirements. Various approaches have been proposed to make CNNs efficient like grouped, shuffled, depth-wise separable convolutions. We study the effectiveness of these techniques on a real-time semantic segmentation architecture like ERFNet for improving runtime by over 5X. We apply these techniques to CNN layers partially or fully and evaluate the testing accuracies on Cityscapes dataset.  We obtain accuracy vs parameters/FLOPs trade offs, giving accuracy scores for models that can run under specified runtime budgets. We further propose a novel training procedure which starts out with a dense convolution but gradually evolves towards a grouped convolution. We show that our proposed training method and efficient architecture design can improve accuracies by over 8% with depthwise separable convolutions applied on the encoder of ERFNet and attaching a light weight decoder. This results in a model which has a 5X improvement in FLOPs while only suffering a 4% degradation in accuracy with respect to ERFNet.