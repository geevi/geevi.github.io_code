+++
title = "Deep Expander Networks: Efficient Deep Networks from Graph Theory"
date = "2018-07-03"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ['''<a href='https://researchweb.iiit.ac.in/~ameya.prabhu/'>Ameya Prabhu</a>''', "Girish Varma", '''<a href="https://faculty.iiit.ac.in/~anoop/">Anoop Namboodiri</a>''']

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
publication = '''<span style='color: orange'>Oral Presentation</span><br/><a href='https://eccv2018.org/'>European Conference on Computer Vision (<strong>ECCV'18</strong>)</a>'''
#publication_short = "ECCV'18"

# Abstract and optional shortened version.
abstract = ""

# Featured image thumbnail (optional)
image_preview = "/img/xnet.png"

# Is this a selected publication? (true/false)
selected = true

bibtex='''@InProceedings{PVN18,
author="Prabhu, Ameya
and Varma, Girish
and Namboodiri, Anoop",
editor="Ferrari, Vittorio
and Hebert, Martial
and Sminchisescu, Cristian
and Weiss, Yair",
title="Deep Expander Networks: Efficient Deep Networks from Graph Theory",
booktitle="Computer Vision -- ECCV 2018",
year="2018",
publisher="Springer International Publishing",
address="Cham",
pages="20--36",
isbn="978-3-030-01261-8"
}
'''

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["model-compression"]

# Links (optional).
#url_pdf = "http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w12/Vallurupalli_Efficient_Semantic_Segmentation_CVPR_2018_paper.pdf" 
url_preprint = "https://arxiv.org/abs/1711.08757"
url_code = "https://github.com/DrImpossible/Deep-Expander-Networks"
#url_dataset = "#"
#url_project = "#"
#url_slides = "#"
#url_video = "#"
url_poster = "/pdfs/ECCV18.pdf"
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

Efficient CNN designs like ResNets and DenseNet were proposed to improve accuracy vs efficiency trade-offs. They essentially increased the connectivity, allowing efficient information flow across layers. Inspired by these techniques, we propose to model connections between filters of a CNN using graphs which are simultaneously sparse and well connected. Sparsity results in efficiency while well connectedness can preserve the expressive power of the CNNs. We use a well-studied class of graphs from theoretical computer science that satisfies these properties known as Expander graphs. Expander graphs are used to model connections between filters in CNNs to design networks called X-Nets. We present two guarantees on the connectivity of X-Nets: Each node influences every node in a layer in logarithmic steps, and the number of paths between two sets of nodes is proportional to the product of their sizes. We also propose efficient training and inference algorithms, making it possible to train deeper and wider X-Nets effectively. 
Expander based models give a 4% improvement in accuracy on MobileNet over grouped convolutions, a popular technique, which has the same sparsity but worse connectivity. X-Nets give better performance trade-offs than the original ResNet and DenseNet-BC architectures. We achieve model sizes comparable to state-of-the-art pruning techniques using our simple architecture design, without any pruning. We hope that this work motivates other approaches to utilize results from graph theory to develop efficient network architectures.
