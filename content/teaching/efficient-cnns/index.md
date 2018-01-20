+++
# Date this page was created.
date = "2018-01-01"

# Project title.
title = "Efficient CNNs"

# Project summary to display on homepage.
summary = "Surveying Deep learning methods used in Reinforcement Learning"

# Optional image to display on homepage (relative to `static/img/` folder).
#image_preview = "bubbles.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["deep-learning"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
#image = "headers/bubbles-wide.jpg"
#caption = "My caption :smile:"

+++


Deep Neural Networks, while being unreasonably effective for several vision tasks, have their usage limited by the computational and memory requirements, both during training and inference stages. Analyzing and improving the connectivity patterns between layers of a network has resulted in several compact architectures like GoogleNet, ResNet and DenseNet-BC. We survey the most recent developments giving CNN architectures with better error vs resourse (parameters/FLOPs/energy/memory/fps) tradeoffs.

We also plan to learn how to do fast implementations of CNNs in existing processing architectures. Most important processor currently is the GPU. Hence we plan to learn some amount of GPU programming as well.

## Schedule

Every week we meet for 3 hrs. Broadly it will be divided in to:

- 1 hr will be spent on basics and pre 2017 techniques
- 1 hr on more recent techniques or theory
- 1 hr on GPU programming (also some thing about FPGAs or general hardware?)

## Papers

The topics covered can be broadly classified into following. It is reccomended that each participant take one topic and read all papers related to it. If there are too many in a particular topic, we can find some way to share the load.

### Explicit Compression Techniques

- Trained Pruning and Quantization : https://arxiv.org/abs/1510.00149
- Low Rank and Sparse Approximations : http://ieeexplore.ieee.org/document/8099498/
- Binarized Networks : http://allenai.org/plato/xnornet/

### Efficient CNN Designs

- Grouped Convolutions : 
    - https://ikhlestov.github.io/pages/machine-learning/convolutions-types/
    - https://blog.yani.io/filter-group-tutorial/
- Depthwise Seperable Convolutions (MobileNet)
    - https://arxiv.org/abs/1704.04861
- ResNext
    - https://arxiv.org/abs/1611.05431
- DenseNet
    - https://arxiv.org/abs/1608.06993
- ShuffleNet
    - https://arxiv.org/abs/1707.01083
- Deep Expander Nets
    - https://arxiv.org/abs/1711.08757
- ZeroFLOP operation
    - https://arxiv.org/abs/1711.08141
- Block Sparse GPU Kernels
    - https://blog.openai.com/block-sparse-gpu-kernels/
- Capsule Network
    - https://arxiv.org/abs/1710.09829
- FractalNet
    - https://arxiv.org/abs/1605.07648
- MEC (ICML '17)
    - http://proceedings.mlr.press/v70/cho17a/cho17a.pdf
- Adaptive Neural Networks (ICML '17)
    - http://proceedings.mlr.press/v70/bolukbasi17a/bolukbasi17a.pdf
- Wraped Convolutions (ICMl '17)
    - http://proceedings.mlr.press/v70/henriques17a/henriques17a.pdf

### Architecture Search

- NasNet
    - https://research.googleblog.com/2017/11/automl-for-large-scale-image.html
    - https://arxiv.org/abs/1707.07012
-  Hierarchical Representations for Efficient Architecture Search
    - https://arxiv.org/abs/1711.00436
-  Progressive Neural Architecture Search
    - https://arxiv.org/abs/1712.00559
- CondenseNet
    - https://arxiv.org/abs/1711.09224


### GPU Programming

- Follow course notes : http://courses.cms.caltech.edu/cs179/

### Theory for CNNs
- Follow some papers from : https://stats385.github.io/readings

## Schedule 

- CNN Introduction and Survey | Depthwise Seperarable Convolutions (Inception, Xception, MobileNet) | GPU 1
- Pruning and Quantization Introduction | Residual and Dense Connections (ResNet, ResNext and DenseNet) | GPU 2
- Architecture Search Introduction
- ShuffleNet


## Students
- Ameya


