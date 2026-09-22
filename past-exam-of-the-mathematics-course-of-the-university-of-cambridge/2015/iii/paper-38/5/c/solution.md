<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an explicit [algorithm](../../../../../../algorithm.md), keep an unnormalized residual $R$, initially $A$, whose row and column sums all equal a common mass $\tau$, initially one. While $\tau>0$, find a [perfect matching](../../../../../../perfect-matching.md) in its positive support, form its [permutation matrix](../../../../../../permutation-matrix.md) $P$, and subtract $\alpha P$, where $\alpha$ is the smallest selected entry. Record $(\alpha,P)$ and replace $\tau$ by $\tau-\alpha$.

If the residual mass is positive, the same proof of the [Hall marriage theorem](../../../../../../hall-s-marriage-theorem.md) condition applies after division by $\tau$. Every subtraction removes at least one positive entry and creates no new positive entries. Before the last subtraction, any positive-mass residual has at least $n$ positive entries; the last step removes all its entries. If $r$ is the initial number of positive entries, then

$$
\boxed{k\leq r-n+1\leq n^2-n+1.}
$$

Since the residual ultimately vanishes, summing the recorded subtractions gives $A=\sum\alpha_iP_i$, and the row sums give $\sum\alpha_i=1$.

A [perfect matching](../../../../../../perfect-matching.md) can be found by at most $n$ searches for an [augmenting path in a matching](../../../../../../augmenting-path-in-a-matching.md), each costing $O(n^2)$ in a graph with at most $n^2$ edges. Thus each iteration costs $O(n^3)$, including forming the support and updating the residual, and there are $O(n^2)$ iterations. Hence

$$
\boxed{\text{running time }O(n^5)\text{ arithmetic/comparison operations}.}
$$

This bound uses exact real arithmetic. For rational input, a common denominator lets all residual subtractions be performed on integers of polynomial bit length, giving a polynomial bit-time implementation as well.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
