<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Poisson random measure](../../../../../../poisson-random-measure.md) with intensity the [sigma-finite measure](../../../../../../sigma-finite-measure.md) $\mu$ is a random nonnegative integer-valued measure $M$ such that, for each outcome outside a single null set, $A\mapsto M(A)$ is countably additive, and for each measurable $A$, $M(A)$ is a measurable [random variable](../../../../../../random-variable-split.md). For every measurable $A$ with $\mu(A)<\infty$,

$$
\mathbb P(M(A)=j)=e^{-\mu(A)}\frac{\mu(A)^j}{j!},\qquad j=0,1,2,\ldots;
$$

and for every finite collection of pairwise disjoint finite-intensity measurable sets, their counts are [independent random variables](../../../../../../independent-random-variables.md). These are integer-valued counts, with possible value infinity on infinite-intensity sets. In particular $\mu(A)=0$ implies $M(A)=0$ [almost surely](../../../../../../almost-sure-convergence.md). The intensity identity is $\mathbb EM(A)=\mu(A)$, also in the extended sense.

For completeness, choose an increasing finite-intensity exhaustion $E_m\uparrow E$. Each $M(E_m)$ is finite [almost surely](../../../../../../almost-sure-convergence.md), simultaneously for all $m$, so $M$ is a [sigma-finite measure](../../../../../../sigma-finite-measure.md) [almost surely](../../../../../../almost-sure-convergence.md). If $\mu(A)=\infty$, then $\mu(A\cap E_m)\to\infty$, and for any fixed integer $K$,

$$
\mathbb P(M(A)\leq K)\leq\mathbb P(M(A\cap E_m)\leq K)
=e^{-\mu(A\cap E_m)}\sum_{j=0}^K\frac{\mu(A\cap E_m)^j}{j!}\longrightarrow0.
$$

Hence $M(A)=\infty$ [almost surely](../../../../../../almost-sure-convergence.md). Independence for counts on arbitrary disjoint measurable sets follows by this exhaustion; an infinite count is a constant extended value. This convention completes the definition on a general [measurable space](../../../../../../measurable-space.md), not just on bounded subsets of Euclidean space.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
