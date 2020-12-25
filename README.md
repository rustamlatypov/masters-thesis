# Coloring Sparse Graphs with 3 Colors in the Massively Parallel Computation (MPC) Model Using Strongly Sublinear Memory

Masters's thesis at Aalto University.

Developed during June - December, 2020.

## Abstract

The question of what problems can be solved, and how efficiently, has always been at the core of theoretical computer science. One such fundamental problem is graph coloring; it is well researched and has numerous applications in areas of computer science such as scheduling and pattern matching. \\

The challenges faced when designing graph coloring algorithms are dictated by the underlying graph family, the number of colors allowed, and the model of computation. In this work we consider the graph family of trees and the distributed Massively Parallel Computation (MPC) model, introduced by Karloff et al. \cite{karloff}. Our contribution to the field of distributed computing is a deterministic strongly sublinear MPC algorithm for 3-coloring unbounded degree trees with $n$ nodes in $O(\log \log n)$ time. To the best of our knowledge, this is the current state-of-the-art algorithm, improving on the work of Ghaffari et al. \cite{ghaffari}. It is loosely based on two previous works by Brandt et al. \cite{sparce,sirocco}. \\

Before computing a 3-coloring, our algorithm partitions the input tree into disjoint node sets $H_1,H_2,\dots,H_l$, in $O(\log \log n)$ time. For each node $v \in H_i$, it holds that $v$ has at most two neighbors in the set $\bigcup_{j=i}^l H_j$. We consider this partitioning in and of itself an important contribution, since it has the potential of being a useful subroutine in future algorithms. For example, a similar technique was used by Chang et al. \cite{chang} in their seminal paper to establish an important time hierarchy theorem for the distributed LOCAL model on trees. 


## Author

[Rustam Latypov](mailto:rustam.latypov@aalto.fi)


## Acknowledgements

Supervisor and instructor of Bachelor's thesis: [Jara Uitto](mailto:jara.uitto@aalto.fi)



