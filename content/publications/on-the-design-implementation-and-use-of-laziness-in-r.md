+++
title = "On the Design, Implementation, and Use of Laziness in R"
date = 2019-10-06T00:00:00-04:00
draft = false

[taxonomies]
categories = ["Publications"]
tags = ["R", "Delayed Evaluation", "Lazy Evaluation"]

[extra]
authors = ["Aviral Goel", "Jan Vitek"]
doi = "10.1145/3360579"
pdf = "on-the-design-implementation-and-use-of-laziness-in-r.pdf"

[extra.talk]
youtube = "https://youtu.be/qLxz9HPP6wI"

[extra.venue]
name = "OOPSLA"
year = 2019
url = "https://2019.splashcon.org/track/splash-2019-oopsla"

[extra.references]
#acmdl = "https://dl.acm.org/doi/10.1145/3360579"
#arxiv = "1909.08958/"

[extra.artifact]
zenodo = "https://zenodo.org/record/3369573#.XaC2c-aYVhE"
functional = "https://2019.splashcon.org/details/splash-2019-Artifacts/25/On-The-Design-Implementation-and-Use-of-Laziness-in-R"
reusable = "https://2019.splashcon.org/details/splash-2019-Artifacts/25/On-The-Design-Implementation-and-Use-of-Laziness-in-R"
available = "https://2019.splashcon.org/details/splash-2019-Artifacts/25/On-The-Design-Implementation-and-Use-of-Laziness-in-R"

[extra.citation]
bibtex='''
@article{10.1145/3360579,
         author = {Goel, Aviral and Vitek, Jan},
         title = {On the Design, Implementation, and Use of Laziness in R},
         year = {2019},
         volume = {3},
         number = {OOPSLA},
         doi = {10.1145/3360579},
         journal = {Proc. ACM Program. Lang.}
}
'''
+++

The R programming language has been lazy for over twenty-five years. This paper presents a review of the design and implementation of call-by-need in R, and a data-driven study of how generations of programmers have put laziness to use in their code. We analyze 16,707 packages and observe the creation of 270.9 B promises. Our data suggests that there is little supporting evidence to assert that programmers use laziness to avoid unnecessary computation or to operate over infinite data structures. For the most part R code appears to have been written without reliance on, and in many cases even knowledge of, delayed argument evaluation. The only significant exception is a small number of packages which leverage call-by-need for meta-programming.
