<h1 id="b/8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Azuma's inequality](../../../../../azuma-s-inequality.md) states that if $(M_i)_{i=0}^m$ is a [martingale](../../../../../martingale-split.md) with $|M_i-M_{i-1}|\le1$ almost surely, then for $t\ge0$,

$$
P(|M_m-M_0|\ge t)\le2\exp(-t^2/(2m)).
$$

For independent product coordinates $Z_1,\ldots,Z_m$, expose them successively and set $M_i=E[f(Z)\mid Z_1,\ldots,Z_i]$. If changing one coordinate changes $f$ by at most one, the possible conditional means at that exposure have [diameter](../../../../../diameter.md) at most one, by averaging the same remaining independent coordinates. Therefore the [martingale](../../../../../martingale-split.md) increments have absolute value at most one. It follows that

$$
\boxed{P(|f(Z)-Ef(Z)|\ge t)\le2\exp(-t^2/(2m))}.
$$

For coordinate bounds $c_i$, the same argument gives denominator $2\sum_i c_i^2$. The argument extends to arbitrary independent measurable coordinates for an [integrable function](../../../../../lebesgue-integrable-function.md) with these bounds, rather than requiring finite state sets.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
