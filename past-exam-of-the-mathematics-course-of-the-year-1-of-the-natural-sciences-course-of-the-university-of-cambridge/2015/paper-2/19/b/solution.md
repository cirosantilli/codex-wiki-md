<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $\mathcal L=-\sum_i x_i\log x_i-\lambda(\sum_i x_i-1)$. Differentiating with respect to each positive $x_i$ gives

$$
-\log x_i-1-\lambda=0.
$$

Every $x_i$ is therefore equal; normalization forces

$$
\boxed{x_i=\frac1n\quad\text{for all }i},\qquad
\boxed{f_{\rm stationary}=\log n}.
$$

The [Hessian matrix](../../../../../hessian-matrix.md) of $f$ is diagonal with entries $-1/x_i$, so its quadratic form is strictly negative for every nonzero perturbation. In particular it is negative along the tangent space $\sum_i\delta x_i=0$, making this the unique global maximum on the positive [probability simplex](../../../../../probability-simplex.md). This is the [maximum entropy distribution on a finite set](../../../../../maximum-entropy-distribution-on-a-finite-set.md), using natural logarithms.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
