<h1 id="19/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $p\leq0$, the terms $k^{-p}$ do not tend to zero, so the series diverges. For $p>0$, group the positive terms into the dyadic blocks $2^j\leq k<2^{j+1}$. Each block contains $2^j$ terms, and monotonicity gives

$$
2^{-p}\,2^{j(1-p)}\leq
\sum_{k=2^j}^{2^{j+1}-1}k^{-p}
\leq2^{j(1-p)}.
$$

When $p>1$, the upper bounds form a convergent [geometric series](../../../../../geometric-series.md) with ratio $2^{1-p}<1$, proving convergence. When $0<p\leq1$, the lower bounds do not tend to zero, so infinitely many blocks each make a nonvanishing contribution and the sum diverges. Thus the [p-series](../../../../../p-series.md) criterion is

$$
\boxed{\sum_{k=1}^{\infty}k^{-p}\text{ converges exactly when }p>1.}
$$

This dyadic comparison is the mechanism of the [Cauchy condensation test](../../../../../cauchy-condensation-test.md). In particular $p=1$ is the divergent [harmonic series](../../../../../harmonic-series.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
