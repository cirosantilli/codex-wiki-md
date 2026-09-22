<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [mean](../../../../../expected-value-split.md) of a shape-rate [gamma distribution](../../../../../gamma-distribution.md) is shape divided by rate. Hence the [posterior mean](../../../../../posterior-mean.md) is

$$
\mathbb E(\theta\mid x)=\frac{a+n\overline x}{b+n}
=\frac b{b+n}\frac ab+\frac n{b+n}\overline x.
$$

Both weights are positive and sum to one. This is a [convex combination](../../../../../convex-combination.md) of the [prior mean](../../../../../prior-mean.md) and the [sample mean](../../../../../sample-mean.md), proving

$$
\boxed{\min\{a/b,\overline x\}\leq\mathbb E(\theta\mid x)\leq\max\{a/b,\overline x\}.}
$$

For $n\geq1$ it lies strictly between them if the two means differ, and equals both if they agree. The rate $b$ acts as the prior weight relative to the $n$ observed exposure units.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
