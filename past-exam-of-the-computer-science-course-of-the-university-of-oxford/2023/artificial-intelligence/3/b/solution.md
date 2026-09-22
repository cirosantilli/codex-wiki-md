<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use one variable $Y_j$ per item, with [constraint domain](../../../../../constraint-domain.md) $\{1,\ldots,n\}$. Its value is the recipient agent. Every assignment automatically allocates each item exactly once, so separate coverage and disjointness constraints are unnecessary.

For every ordered pair $i\ne\ell$, impose

$$
\boxed{\sum_{j=1}^{m}v_{ij}\mathbf1_{\{Y_j=i\}}
\ge
\sum_{j=1}^{m}v_{ij}\mathbf1_{\{Y_j=\ell\}}.}
$$

Here $\mathbf1$ is an [indicator function](../../../../../indicator-function.md). The constraint involves every $Y_j$ with $v_{ij}\ne0$; one may formally give it scope $\{Y_1,\ldots,Y_m\}$, since zero coefficients make the other variables irrelevant. These constraints state [envy-free allocation](../../../../../envy-free-allocation.md) using the comparing agent's [additive valuation](../../../../../additive-valuation.md) on both sides. In contrast to part (a), they generally involve more than two variables.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
