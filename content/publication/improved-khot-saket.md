+++
title = "Reducing uniformity in Khot-Saket hypergraph coloring hardness reductions"
date = "2015-05-10"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = [ "Girish Varma"]


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
publication = "*Chicago J. Theor. Comput. Sci*."
publication_short = "*Chicago J. Theor. Comput. Sci*"

# Abstract and optional shortened version.
abstract = ""

# Featured image thumbnail (optional)
image_preview = ""

# Is this a selected publication? (true/false)
selected = true

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["hardness"]

# Links (optional).
#url_pdf =  "https://doi.org/10.1016/j.jtbi.2012.06.017"
url_preprint = "https://arxiv.org/abs/1408.0262"
#url_code = "#"
#url_dataset = "#"
#url_project = "#"
#url_slides = "https://www.dropbox.com/s/mv391tfzysae7ee/slides.pdf?dl=0"
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

In a recent result, Khot and Saket [FOCS 2014] proved the quasi-NP-hardness of coloring a 2-colorable 12-uniform hypergraph with 2(logn)Ω(1) colors. This result was proved using a novel outer PCP verifier which had a strong soundness guarantee. In this note, we show that we can reduce the arity of their result by modifying their 12-query inner verifier to an 8-query inner verifier based on the hypergraph coloring hardness reductions of Guruswami et. al. [STOC 2014]. More precisely, we prove quasi-NP-hardness of the following problems on n-vertex hypergraphs. 

- Coloring a 2-colorable 8-uniform hypergraph with 2(logn)Ω(1) colors. 
- Coloring a 4-colorable 4-uniform hypergraph with 2(logn)Ω(1) colors. 