+++
title="Designing Types for R, Empirically"
date=2020-11-01
draft = false

[taxonomies]
categories = ["Publications"]
tags = ["Type Declarations", "Dynamic Languages", "R"]

[extra]
authors=["Alexi Turcotte", "Aviral Goel", "Filip Křikava", "Jan Vitek"]
doi = "10.1145/3428249"
pdf = "designing-types-for-r-empirically.pdf"

[extra.talk]
youtube = "https://youtu.be/GMrLtYg0VGA"

[extra.venue]
name = "OOPSLA"
year = 2020
url = "https://2020.splashcon.org/track/splash-2020-oopsla"

[extra.references]
acmdl = "https://dl.acm.org/doi/10.1145/3428249"

[extra.artifact]
zenodo = "https://zenodo.org/record/4037278#.X9U4B1OYUUF"
functional = "https://2020.splashcon.org/details/splash-2020-Artifacts/34/Designing-Types-for-R-Empirically"
reusable = "https://2020.splashcon.org/details/splash-2020-Artifacts/34/Designing-Types-for-R-Empirically"
available = "https://2020.splashcon.org/details/splash-2020-Artifacts/34/Designing-Types-for-R-Empirically"

[extra.citation]
bibtex = '''
@article{10.1145/3428249,
         author = {Turcotte, Alexi and
                   Goel, Aviral and
                   K\v{r}ikava, Filip and
                   Vitek, Jan},
         title = {Designing Types for R, Empirically},
         year = {2020},
         volume = {4},
         number = {OOPSLA},
         doi = {10.1145/3428249},
         journal = {Proc. ACM Program. Lang.}
}
'''
+++

The R programming language is widely used in a variety of domains. It was designed to favor an interactive
style of programming with minimal syntactic and conceptual overhead. This design is well suited to data
analysis, but a bad fit for tools such as compilers or program analyzers. In particular, R has no type annotations,
and all operations are dynamically checked at runtime. The starting point for our work are the two questions:
*what expressive power is needed to accurately type R code?* and *which type system is the R community willing to
adopt?* Both questions are difficult to answer without actually experimenting with a type system. The goal of
this paper is to provide data that can feed into that design process. To this end, we perform a large corpus
analysis to gain insights in the degree of polymorphism exhibited by idiomatic R code and explore potential
benefits that the R community could accrue from a simple type system. As a starting point, we infer type
signatures for 25,215 functions from 412 packages among the most widely used open source R libraries. We
then conduct an evaluation on 8,694 clients of these packages, as well as on end-user code from the Kaggle
data science competition website.
