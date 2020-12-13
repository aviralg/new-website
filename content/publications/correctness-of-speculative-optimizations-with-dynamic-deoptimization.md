+++
title="Correctness of Speculative Optimizations with Dynamic Deoptimization"
date=2017-12-01
draft = false

[taxonomies]
categories = ["Publications"]
tags = ["Dynamic Deoptimization", "On-Stack-Replacement", "Speculative Optimizations", "Compiler Correctness"]

[extra]
authors=["Olivier Flückiger", "Gabriel Scherer", "Ming-ho Yee", "Aviral Goel", "Amal Ahmed", "Jan Vitek"]
doi = "10.1145/3158137"
pdf = "correctness-of-speculative-optimizations-with-dynamic-deoptimization.pdf"

[extra.venue]
name = "POPL"
year = 2018
url = "https://popl18.sigplan.org/"

[extra.references]
acmdl = "https://dl.acm.org/doi/10.1145/3158137"
arxiv = "1711.03050/"

[extra.citation]
bibtex = '''
@article{10.1145/3158137,
         author = {Fl\"{u}ckiger, Olivier and
                   Scherer, Gabriel and
                   Yee, Ming-Ho and
                   Goel, Aviral and
                   Ahmed, Amal and
                   Vitek, Jan},
         title = {Correctness of Speculative Optimizations 
                  with Dynamic Deoptimization},
         year = {2017},
         volume = {2},
         number = {POPL},
         doi = {10.1145/3158137},
         journal = {Proc. ACM Program. Lang.}
}
'''
+++

High-performance dynamic language implementations make heavy use of speculative optimizations to achieve speeds close to statically compiled languages. These optimizations are typically performed by a just-in-time compiler that generates code under a set of assumptions about the state of the program and its environment. In certain cases, a program may execute code compiled under assumptions that are no longer valid. The implementation must then deoptimize the program on-the-!y; this entails "nding semantically equivalent code that does not rely on invalid assumptions, translating program state to that expected by the target code, and transferring control. This paper looks at the interaction between optimization and deoptimization, and shows that reasoning about speculation is surprisingly easy when assumptions are made explicit in the program representation. This insight is demonstrated on a compiler intermediate representation, named `sourir`, modeled after the high-level representation for a dynamic language. Traditional compiler optimizations such as constant folding, unreachable code elimination, and function inlining are shown to be correct in the presence of assumptions. Furthermore, the paper establishes the correctness of compiler transformations specific to deoptimization: namely unrestricted deoptimization, predicate hoisting, and assume composition.

