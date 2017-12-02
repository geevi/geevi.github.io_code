+++
title = "Streaming Algorithms for Some Problems in Log-Space"
date = "2010-01-01"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Ajesh Babu", "Nutan Limaye", "Girish Varma"]

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
publication = "* Theory and Applications of Models of Computation (TAMC)*."
publication_short = "*TAMC*"

# Abstract and optional shortened version.
abstract = ""

# Featured image thumbnail (optional)
image_preview = ""

# Is this a selected publication? (true/false)
selected = false

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["streaming"]

# Links (optional).
url_pdf =  "https://link.springer.com/chapter/10.1007/978-3-642-13562-0_10"
url_preprint = "http://arxiv.org/abs/1104.0848"
#url_code = "#"
#url_dataset = "#"
#url_project = "#"
url_slides = "https://www.dropbox.com/s/j7p2enoptwzky25/slides.pdf?dl=0"
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

In this paper, we give streaming algorithms for some problems which are known to be in deterministic log-space, when the number of passes made on the input is unbounded. If the input data is massive, the conventional deterministic log-space algorithms may not run efficiently. We study the complexity of the problems when the number of passes is bounded. 

The first problem we consider is the membership testing problem for deterministic linear languages, DLIN. Extending the recent work of Magniez et al.[11](to appear in STOC 2010), we study the use of fingerprinting technique for this problem. We give the following streaming algorithms for the membership testing of DLIN s: a randomized one pass algorithm that uses O(logn) space (one-sided error, inverse polynomial error probability), and also a p-pass O(n/p)-space deterministic algorithm. We also prove that there exists a language in DLIN, for which any p-pass deterministic algorithm for membership testing, requires Ω(n/p) space. We also study the application of fingerprinting technique to visibly pushdown languages, VPL s. 

The other problem we consider is, given a degree sequence and a graph, checking whether the graph has the given degree sequence, Deg-Seq. We prove that, any p-pass deterministic algorithm that takes as its input a degree sequence, followed by an adjacency list of a graph, requires Ω(n/p) space to decide Deg-Seq. However, using randomness, for a more general input format: degree sequence, followed by a list of edges in any arbitrary order, Deg-Seq can be decided in O(logn) space. We also give a p-pass, O(n/p)-space deterministic algorithm for Deg-Seq.