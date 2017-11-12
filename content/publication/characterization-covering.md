+++
title = "A Characterization of Hard-to-cover CSPs"
date = "2015-08-10"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Amey Bhangale", "Prahladh Harsha", "Girish Varma"]

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
publication = "*Computational Complexity Conference 2015*."
publication_short = "*CCC*"

# Abstract and optional shortened version.


# Featured image thumbnail (optional)
image_preview = ""

# Is this a selected publication? (true/false)
selected = true

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["hardness", "pcps"]

# Links (optional).
#url_pdf =  "https://doi.org/10.1016/j.jtbi.2012.06.017"
url_preprint = "https://arxiv.org/abs/1411.7747"
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
We continue the study of covering complexity of constraint satisfaction problems (CSPs) initiated by Guruswami, Hastad and Sudan [SIAM J. Computing, 31(6):1663--1686, 2002] and Dinur and Kol [In Proc. 28th IEEE Conference on Computational Complexity, 2013]. The covering number of a CSP instance $\phi$, denoted by ν(Φ) is the smallest number of assignments to the variables of $\phi$, such that each constraint of Φ is satisfied by at least one of the assignments. We show the following results regarding how well efficient algorithms can approximate the covering number of a given CSP instance. 

- Assuming a covering unique games conjecture, introduced by Dinur and Kol, we show that for every non-odd predicate P over any constant sized alphabet and every integer K, it is NP-hard to distinguish between P-CSP instances (i.e., CSP instances where all the constraints are of type P) which are coverable by a constant number of assignments and those whose covering number is at least K. Previously, Dinur and Kol, using the same covering unique games conjecture, had shown a similar hardness result for every non-odd predicate over the Boolean alphabet that supports a pairwise independent distribution. Our generalization yields a complete characterization of CSPs over constant sized alphabet Σ that are hard to cover since CSP's over odd predicates are trivially coverable with |Σ| assignments. 

- For a large class of predicates that are contained in the 2k-LIN predicate, we show that it is quasi-NP-hard to distinguish between instances which have covering number at most two and covering number at least Ω(loglogn). This generalizes the 4-LIN result of Dinur and Kol that states it is quasi-NP-hard to distinguish between 4-LIN-CSP instances which have covering number at most two and covering number at least Ω(logloglogn).