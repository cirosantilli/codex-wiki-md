<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $a=s+ib$ with real $s,b$, and first translate the real integration variable by $s$. It remains to integrate $e^{-z^2}$ along the horizontal line $\operatorname{Im}z=b$.

For $b>0$, apply the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) to the rectangle with vertices $-R,R,R+ib,-R+ib$. The [integrand](../../../../../integrand.md) is an [entire function](../../../../../entire-function.md), so

$$
\int_{-R}^{R}e^{-x^2}\,dx-\int_{-R}^{R}e^{-(x+ib)^2}\,dx
$$

is the negative of the two vertical-edge integrals. On either vertical edge, $z=\pm R+iy$ and

$$
|e^{-z^2}|=e^{-R^2+y^2}\leq e^{-R^2+b^2}.
$$

Their combined absolute value is at most $2b e^{-R^2+b^2}$ and tends to zero. The rectangle below the real axis gives the same estimate with $|b|$ when $b<0$; $b=0$ needs no deformation. Absolute convergence follows from $|e^{-(x+ib)^2}|=e^{b^2}e^{-x^2}$. Taking $R\to\infty$ proves the [Gaussian contour translation](../../../../../gaussian-contour-translation.md) identity

$$
\boxed{\int_{-\infty}^{\infty}e^{-(u+a)^2}\,du=\sqrt\pi,\qquad a\in\mathbb C}.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
