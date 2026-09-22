<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For every positive real $r$, a centered [normal](../../../../../../normal-distribution.md) variable of [variance](../../../../../../variance-split.md) $t-s$ has absolute $r$th moment $c_r|t-s|^{r/2}$, where $c_r=\mathbb E|N(0,1)|^r<\infty$. Fix $0<\alpha<1/2$ and choose $r$ large enough that $\alpha<1/2-1/r$. Then

$$
\mathbb E|B_t-B_s|^r=c_r|t-s|^{1+(r/2-1)}.
$$

The [Kolmogorov continuity theorem](../../../../../../kolmogorov-continuity-theorem.md) gives a modification with [Hölder continuity](../../../../../../holder-condition.md) of every exponent less than $(r/2-1)/r=1/2-1/r$, in particular exponent $\alpha$, on each compact interval. This modification and the given continuous [Brownian motion](../../../../../../brownian-motion-split.md) agree almost surely at all rational times; continuity makes them agree everywhere simultaneously. Thus the property holds for the given trajectories, not just for another version.

Take a [countable](../../../../../../countable-set.md) increasing sequence of positive exponents approaching $1/2$, and intersect their probability-one events for every integer time horizon. [Hölder continuity](../../../../../../holder-condition.md) of a larger exponent implies that of every smaller positive exponent on a compact interval, after adjusting the constant. We have therefore proved the simultaneous assertion

$$
\boxed{\text{Almost surely, }B\text{ is locally }\alpha\text{-Hölder for every }0<\alpha<\tfrac12.}
$$

The compact-interval qualification matters: a single uniform Hölder constant on the entire half-line is not being asserted.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
