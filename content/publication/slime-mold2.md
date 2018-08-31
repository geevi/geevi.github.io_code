+++
title = " Physarum Can Compute Shortest Paths"
date = "2012-09-12"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = [" Vincenzo Bonifaci", "Kurt Mehlhorn", "Girish Varma"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference proceedings
# 2 = Journal
# 3 = Work in progress
# 4 = Technical report
# 5 = Book
# 6 = Book chapter
publication_types = ["2"]
# Publication name and optional abbreviated version.
publication = '''<span style='color: orange'>Journal of Theoretical Biology (<strong>JTB</strong>)</span><br/>Symp. of Discrete Algorithms (<strong>SODA</strong>)'''
publication_short = "JTB'12"

# Abstract and optional shortened version.
abstract = ""

# Featured image thumbnail (optional)
image_preview = "/img/physarum.png"

# Is this a selected publication? (true/false)
selected = true

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["physarum-computer"]

# Links (optional).
url_pdf =  "https://doi.org/10.1016/j.jtbi.2012.06.017"
url_preprint = "https://arxiv.org/abs/1106.0423"
#url_code = "#"
#url_dataset = "#"
#url_project = "#"
#url_slides = "https://www.dropbox.com/s/j7p2enoptwzky25/slides.pdf?dl=0"
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
Physarum polycephalum is a slime mold that is apparently able to solve shortest path problems. A mathematical model has been proposed by Tero et al. (Journal of Theoretical Biology, 244, 2007, pp. 553–564) to describe the feedback mechanism used by the slime mold to adapt its tubular channels while foraging two food sources s0 and s1. We prove that, under this model, the mass of the mold will eventually converge to the shortest path of the network that the mold lies on, independently of the structure of the network or of the initial mass distribution. This matches the experimental observations by Tero et al. and can be seen as an example of a “natural algorithm”, that is, an algorithm developed by evolution over millions of years. 

Highlights 
► A standard model for Physarum converges to the shortest path in any network.
► When flow directions stabilize, convergence to the shortest path is fast. 
► Flow directions stabilize in series–parallel networks and Wheatstone networks.
