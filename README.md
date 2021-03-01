# Coloring Sparse Graphs with 3 Colors in the Massively Parallel Computation (MPC) Model Using Strongly Sublinear Memory

Masters's thesis at Aalto University [https://aaltodoc.aalto.fi/handle/123456789/102452].

Developed during June - December, 2020.

## Abstract

The question of what problems can be solved, and how efficiently, has always been at the core of theoretical computer science. One such fundamental problem is graph coloring; it is well researched and has numerous applications in areas of computer science such as scheduling and pattern matching.

The challenges faced when designing graph coloring algorithms are dictated by the underlying graph family, the number of colors allowed, and the model of computation. In this work we consider the graph family of trees and the distributed Massively Parallel Computation (MPC) model, introduced by Karloff et al. [[1]](#1). Our contribution to the field of distributed computing is a deterministic strongly sublinear MPC algorithm for 3-coloring unbounded degree trees with n nodes in O(log log n) time. To the best of our knowledge, this is the current state-of-the-art algorithm, improving on the work of Ghaffari et al. [[2]](#2). It is loosely based on two previous works by Brandt et al. [[3]](#3) [[4]](#4).

Before computing a 3-coloring, our algorithm partitions the input tree into disjoint node sets H_1,H_2,...,H_l, in O(log log n) time. For each node v in H_i, it holds that v has at most two neighbors in the set U_{j=i}^l H_j. We consider this partitioning in and of itself an important contribution, since it has the potential of being a useful subroutine in future algorithms. For example, a similar technique was used by Chang et al. [[5]](#5) in their seminal paper to establish an important time hierarchy theorem for the distributed LOCAL model on trees. 

## References
<a id="1">[1]</a> 
Howard Karloff, Siddharth Suri, and Sergei Vassilvitskii. A model of computation for MapReduce. In Proceedings of the 2010 Annual ACM-SIAM Symposium on Discrete Algorithms (SODA’10), pages 938–948,2010. https://doi.org/10.1137/1.9781611973075.76

<a id="1">[2]</a> 
Mohsen Ghaffari, Christoph Grunau, and Ce Jin. Improved MPC algorithms for MIS, matching, and coloring on trees and beyond. In 34th International Symposium on Distributed Computing (DISC’20), pages 34:1–34:18, 2020. https://arxiv.org/abs/2002.09610v2

<a id="1">[3]</a> 
Sebastian Brandt, Manuela Fischer, and Jara Uitto. Matching and MIS for uniformly sparse graphs in the low-memory MPC model. CoRR, 2018. https://arxiv.org/abs/1807.05374 

<a id="1">[4]</a> 
Sebastian Brandt, Manuela Fischer, and Jara Uitto. Breaking the linear-memory barrier in MPC: Fast MIS on trees with strongly sublinear memory. In Structural Information and Communication Complexity (SIROCCO’19), pages 124–138, 2019. https://doi.org/10.1007/978-3-030-24922-9_9

<a id="1">[5]</a> 
Yi-Jun Chang and Seth Pettie. A time hierarchy theorem for the LOCAL model. In IEEE 58th Annual Symposium on Foundations of Computer Science (FOCS’17), pages 156–167, 2017. https://doi.org/10.1109/FOCS.2017.23

## Author

[Rustam Latypov](mailto:rustam.latypov@aalto.fi)


## Acknowledgements

Supervisor and instructor of Masters's thesis: [Jara Uitto](mailto:jara.uitto@aalto.fi)



