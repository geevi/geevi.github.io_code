+++
title = "Improved Visual Relocalization by Discovering Anchor Points"
date = "2018-07-01"

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
publication = '''<span style='color: orange'>Spotlight Presentation</span><br/>British Machine Vision Conference (<strong>BMVC'18</strong>)'''
#publication_short = "In *ACPR*"

bibtex='''
@inproceedings{SVJ18,
  author    = {Soham Saha and
               Girish Varma and
               C. V. Jawahar},
  title     = {Improved Visual Relocalization by Discovering Anchor Points},
  booktitle = {British Machine Vision Conference 2018, {BMVC} 2018, Northumbria University,
               Newcastle, UK, September 3-6, 2018},
  pages     = {164},
  year      = {2018},
  url       = {http://bmvc2018.org/contents/papers/0962.pdf}
}
'''
# Abstract and optional shortened version.
abstract = ""

# Featured image thumbnail (optional)
image_preview = "/img/achor.png"

# Is this a selected publication? (true/false)
selected = true

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["auto-nav"]

# Links (optional).
url_pdf = "http://bmvc2018.org/contents/papers/0962.pdf" 
url_preprint = "https://arxiv.org/abs/1811.04370"
url_code = "https://github.com/Soham0/Improved-Visual-Relocalization"
#url_dataset = "#"
#url_project = "#"
url_slides = "/pdfs/BMVC_2018_Spotlight.pdf"
#url_video = "#"
url_poster = "/pdfs/BMVC_2018_Poster.pdf"
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
We address the visual relocalization problem of predicting the location and camera
orientation or pose (6DOF) of the given input scene. We propose a method based on how
humans determine their location using the visible landmarks. We define anchor points
uniformly across the route map and propose a deep learning architecture which predicts
the most relevant anchor point present in the scene as well as the relative offsets with
respect to it. The relevant anchor point need not be the nearest anchor point to the ground
truth location, as it might not be visible due to the pose. Hence we propose a multi task
loss function, which discovers the relevant anchor point, without needing the ground truth
for it. We validate the effectiveness of our approach by experimenting on Cambridge
Landmarks (large scale outdoor scenes) as well as 7 Scenes (indoor scenes) using various
CNN feature extractors. Our method improves the median error in indoor as well as
outdoor localization datasets compared to the previous best deep learning model known
as PoseNet (with geometric re-projection loss) using the same feature extractor. We
improve the median error in localization in the specific case of Street scene, by over 8m.