+++
title = "Cityscale Road Audit System using Deep Learning"
date = "2018-05-01"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Sudhir Kumar Reddy", "Girish Varma", '''<a href="https://faculty.iiit.ac.in/~jawahar/">C V Jawahar</a>''']

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
publication = '''<span style='color: orange'>JTCF Novel Technology paper award Finalist</span>
<br/>International Conference on Intelligent Robots (<strong>IROS'18</strong>)'''
#publication_short = "In *ACPR*"

bibtex='''
@inproceedings{YVJ18,
  author    = {Sudhir Yarram and
               Girish Varma and
               C. V. Jawahar},
  title     = {City-Scale Road Audit System using Deep Learning},
  booktitle = {International Conference on Intelligent Robots and Systems (IROS), Madrid, Spain, 2018},
  year      = {2018}
}
'''

# Abstract and optional shortened version.
abstract = ""

# Featured image thumbnail (optional)
image_preview = "/img/audit.png"

# Is this a selected publication? (true/false)
selected = true

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["auto-nav"]

# Links (optional).
#url_pdf = "http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w12/Vallurupalli_Efficient_Semantic_Segmentation_CVPR_2018_paper.pdf" 
#url_preprint = "https://arxiv.org/abs/1711.08757"
url_code = "https://github.com/Sudhir11292rt/City-scale-Road-Audit"
url_dataset = "http://cvit.iiit.ac.in/images/Projects/city-scale-roadaudit/release_version_v1.zip"
url_project = "http://cvit.iiit.ac.in/research/projects/cvit-projects/city-scale-road-audit"
url_slides = "/pdfs/IROS18-slides.pdf"
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
Road networks in cities are massive and is a critical component of mobility. Fast response to defects, that can occur not only due to regular wear and tear but also because of extreme events like storms, is essential. Hence there is a need for an automated system that is quick, scalable and cost-effective for gathering information about defects. We propose a system for city-scale road audit, using some of the most recent developments in deep learning and semantic segmentation. For building and benchmarking the system, we curated a dataset which has annotations required for road defects. However, many of the labels required for road audit have high ambiguity which we overcome by proposing a label hierarchy. We also propose a multi-step deep learning model that segments the road, subdivide the road further into defects, tags the frame for each defect and finally localizes the defects on a map gathered using GPS. We analyze and evaluate the models on image tagging as well as segmentation at different levels of the label hierarchy.
