<h1 id="27i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [busy-period branching equation](../../../../../../busy-period-branching-equation.md), during the first service of a [busy period](../../../../../../busy-period.md), every arriving customer initiates a subtree of further work. The independence and stationary increments of the [Poisson process](../../../../../../poisson-process.md), together with independent services, give the distributional recursion

$$
B_k\overset d=S_k+\sum_{j=1}^{N(S_k)}B_{k,j},
$$

where conditional on $S_k=s$, $N(S_k)$ is Poisson with mean $\lambda s$, and the descendant busy periods are independent copies of $B_k$. One may explore these subtrees in order; the server's total workload is unchanged by that ordering. Consequently, wherever the [moment-generating functions](../../../../../../moment-generating-function.md) are finite,

$$
\phi_{B_k}(\theta)=\mathbb E\!\left[e^{\theta S_k}
\exp\{\lambda S_k(\phi_{B_k}(\theta)-1)\}\right]
=\boxed{\phi_{S_k}(\theta+\lambda(\phi_{B_k}(\theta)-1))}.
$$

For $\lambda<\mu$, this identity in particular holds in a sufficiently small neighbourhood of zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27I](../../27i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
