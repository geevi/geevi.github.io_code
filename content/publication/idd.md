+++
title = "IDD: A Dataset for exploring problems in Autonomous Navigation in Unconstrained Environments"
date = "2018-10-01"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = [
    "Girish Varma", 
    "Anbumani Subramanian",
    '''<a href="https://faculty.iiit.ac.in/~anoop/">Anoop Namboodiri</a>''',
    '''<a href='http://cseweb.ucsd.edu/~mkchandraker/'>Manmohan Chandraker</a>''',
    '''<a href="https://faculty.iiit.ac.in/~jawahar">C V Jawahar</a>'''
]

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
publication = '''<a href='https://wacv2019.org/'>IEEE Winter Conference on Applications of Computer Vision (<strong>WACV'19</strong>)</a>'''
#publication_short = "ECCV'18"

# Abstract and optional shortened version.
abstract = ""

# Featured image thumbnail (optional)
image_preview = "/img/idd.jpg"

# Is this a selected publication? (true/false)
selected = true

bibtex= ''' 
@inproceedings{anue,
  title={IDD: A Dataset for Exploring Problems of Autonomous Navigation in Unconstrained Environments},
  author={Varma, Girish and Subramanian, Anbumani and Namboodiri, Anoop and Chandraker, Manmohan and Jawahar, CV.},
  booktitle={2019 IEEE Winter Conference on Applications of Computer Vision (WACV)},
  year={2019},
  organization={IEEE}
}'''

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
projects = ["auto-nav"]

# Links (optional).
#url_pdf = "http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w12/Vallurupalli_Efficient_Semantic_Segmentation_CVPR_2018_paper.pdf" 
#url_preprint = "https://arxiv.org/abs/1711.08757"
#url_code = "https://github.com/DrImpossible/Deep-Expander-Networks"
url_dataset = "http://cvit.iiit.ac.in/scene-understanding-challenge-2018/"
url_project = "http://cvit.iiit.ac.in/scene-understanding-challenge-2018/"
#url_slides = "#"
#url_video = "#"
#url_poster = "/pdfs/ECCV18.pdf"
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
While several datasets for autonomous navigation have become available in recent years, they tend to focus on structured driving environments. This usually corresponds to well-delineated infrastructure such as lanes, a small number of well-defined categories for traffic participants, low variation in object or background appearance and strict adherence to traffic rules. We propose IDD, a novel dataset for road scene understanding in unstructured environments where the above assumptions are largely not satisfied. It consists of 10,004 images, finely annotated with 34 classes collected from 182 drive sequences on Indian roads. The label set is expanded in comparison to popular benchmarks such as Cityscapes, to account for new classes. It also reflects label distributions of road scenes significantly different from existing datasets, with most classes displaying greater within-class diversity.Consistent with real driving behaviors, it also identifies new classes such as drivable areas besides the road. We propose a new four-level label hierarchy, which allows varying degrees of complexity and opens up possibilities for new training methods. Our empirical study provides an in-depth analysis of the label characteristics. State-of-the-art methods for semantic segmentation achieve much lower accuracies on our dataset, demonstrating its distinction compared to Cityscapes. Finally, we propose that our dataset is an ideal opportunity for new problems such as domain adaptation, few-shot learning and behavior prediction in road scenes.
