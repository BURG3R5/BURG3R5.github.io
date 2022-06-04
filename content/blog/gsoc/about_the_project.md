+++
title = "About the Project"
subtitle = "A quick little glance into the project I'll be working on"
date = 2022-06-04

["taxonomies"]
tags = ["gsoc", "matrix", "python"]
+++

In this project I will implement, in particular, the keyword search scheme outlined in a _Demertzis et al._ paper titled [“Fast Searchable Encryption with Tunable Locality"](http://idemertzis.com/Papers/sigmod17.pdf).

I will achieve this by creating a Python library that exposes methods to create, update and search on encrypted indices stored in content repositories in a Matrix homeserver.

As a part of the project, I will be demonstratively integrating the library into an existing Matrix client. Additionally, I will submit results of preliminary performance evaluation.

#### Goals

In this project I intend to:

1. Implement the keyword search SSE scheme outlined in the aforementioned _Demertzis et al._ paper. 
2. Create encrypted indices of a few public Matrix rooms. 
3. Implement an updation procedure for the above SSE i.e. provide a way to add new messages/documents to the encrypted index. 
4. Integrate the project into a suitable client. 
5. Perform performance evaluation of the created library.

#### Deliverables

* A Python library that exposes methods to create, update and search on encrypted indices.
* Demonstrative integration into a suitable Matrix client. 
* Complete documentation (comments and website) for the library and example codes. 
* Preliminary performance analysis results. 
* Weekly blogs on project progress. 
* GSoC end project report.

#### Pre-GSoC Code

In order to understand the paper and the project idea in the best way possible, I implemented a sort of MVP of this project before writing my proposal for this project. It helped me gain much insight into the project idea and also helped me set milestones. The code is available [here](http://github.com/BURG3R5/sse-experiments). Included are tests, in which both keyword and phrase search are run over 500 messages exported from the official GSoC Matrix room ([#gsoc:matrix.org](http://matrix.to/#/#gsoc:matrix.org)).
