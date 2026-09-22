<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Choose $n\geq1$ as in part (i). Since distances between iterates are nondecreasing, the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
d(\phi x,\phi y)\leq d(\phi^{(n)}x,\phi^{(n)}y)
\leq d(x,y)+d(x,\phi^{(n)}x)+d(y,\phi^{(n)}y)<d(x,y)+2\epsilon.
$$

Letting $\epsilon\downarrow0$ and combining with the given reverse bound proves that $\phi$ is an [isometry](../../../../../isometry.md):

$$
\boxed{d(\phi x,\phi y)=d(x,y)\quad(x,y\in X)}.
$$

For surjectivity, fix $x\in X$ and use part (i) with $y=x$ and $\epsilon=1/k$ to choose $n_k\geq1$ satisfying $d(x,\phi^{(n_k)}x)<1/k$. Put $z_k=\phi^{(n_k-1)}x$, interpreting $\phi^{(0)}$ as the identity. By [sequential compactness](../../../../../sequentially-compact-space.md), a [convergent subsequence](../../../../../convergent-subsequence.md) satisfies $z_{k_j}\to z\in X$. The assumed [continuity](../../../../../continuous-function.md) yields

$$
\phi z=\lim_j\phi z_{k_j}=\lim_j\phi^{(n_{k_j})}x=x.
$$

Thus every $x$ has a preimage, and $\boxed{\phi\text{ is surjective}}$. If $X$ is empty, both conclusions hold vacuously. This proves the [distance-increasing self-map theorem for sequentially compact metric spaces](../../../../../distance-increasing-self-map-theorem-for-sequentially-compact-metric-spaces.md).

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [c](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
