<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a measurable $A$ with $(\mu+\nu)(A)<\infty$, independence of the two [Poisson random measures](../../../../../../poisson-random-measure.md) gives

$$
\mathbb P((\Phi+\Psi)(A)=k)=\sum_{j=0}^k e^{-\mu(A)}\frac{\mu(A)^j}{j!}e^{-\nu(A)}\frac{\nu(A)^{k-j}}{(k-j)!}
=e^{-(\mu+\nu)(A)}\frac{((\mu+\nu)(A))^k}{k!}.
$$

Thus its count has the [Poisson distribution](../../../../../../poisson-distribution.md) with the summed parameter. If $A_1,\ldots,A_m$ are disjoint, the variables within each family of counts are [independent](../../../../../../independent-random-variables.md), and independence of $\Phi$ and $\Psi$ makes the two families [independent](../../../../../../independent-random-variables.md) of each other. Hence the pairs $(\Phi(A_j),\Psi(A_j))$, and therefore their sums, are [independent](../../../../../../independent-random-variables.md) over $j$.

Adding sample counting measures preserves countable additivity. The definition in (a) therefore proves

$$
\boxed{\Phi+\Psi\text{ is a Poisson random measure of intensity }\mu+\nu.}
$$

This proves the required [Superposition theorem for Poisson point processes](../../../../../../superposition-theorem-for-poisson-point-processes.md) directly from count distributions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
