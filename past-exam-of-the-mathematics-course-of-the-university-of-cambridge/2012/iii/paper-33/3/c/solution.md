<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret the second process as an [independent](../../../../../../independent-random-variables.md) copy of the unit-rate [Poisson process](../../../../../../poisson-process.md). First, the sums are finite almost surely. On $[0,1]$ there are finitely many arrivals, none at $0$, so their inverse-square contributions are finite. On $[1,\infty)$,

$$
\mathbb E\sum_{Z_i\geq1}Z_i^{-2}=\int_1^\infty z^{-2}\,dz=1.
$$

For completeness, this [expectation](../../../../../../expected-value.md) identity follows first for nonnegative simple functions from $\mathbb E N(A)=|A|$, and then for all nonnegative measurable functions by [monotone convergence](../../../../../../monotone-convergence-theorem.md). Thus no unproved Poisson-integral formula is needed, and the tail sum is finite almost surely.

By (b), merging the two processes produces a rate-$2$ [Poisson process](../../../../../../poisson-process.md) with arrival times $V_i$. Its rescaled arrivals $2V_i$ form a unit-rate [Poisson process](../../../../../../poisson-process.md): for a measurable set $A$, their count is the merged count on $A/2$, with parameter $2|A/2|=|A|$, and disjoint-set independence is preserved. Consequently

$$
X+Y=\sum_iV_i^{-2}=4\sum_i(2V_i)^{-2}\ \stackrel{d}{=}\ 4X.
$$

Therefore **$\boxed{c=4}$**. This is the scaling of an [inverse-power sum over Poisson arrivals](../../../../../../inverse-power-sum-over-poisson-arrivals.md) with exponent $2$.

The PDF does not explicitly repeat the second process's rate. If that rate were $\rho$ rather than $1$, the same count argument would give $X+Y\stackrel d=(1+\rho)^2X$. The numerical value $4$ uses the intended independent-unit-rate-copy interpretation.

## ↑ Ancestors (11)

1. [C](../c.md)
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
