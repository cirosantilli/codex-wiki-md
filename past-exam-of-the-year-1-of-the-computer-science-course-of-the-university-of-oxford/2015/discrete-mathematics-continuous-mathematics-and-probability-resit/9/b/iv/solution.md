<h1 id="9/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

By the density formula for [expected value](../../../../../../expected-value-split.md),

$$
\mathbb E[X]=\int_0^\infty x^2e^{-x^2/2}\,dx.
$$

For the standard [normal distribution](../../../../../../normal-distribution.md), the integrand in the second [moment](../../../../../../moment.md) is even, so

$$
\mathbb E[Z^2]=\frac1{\sqrt{2\pi}}\int_{-\infty}^{\infty}z^2e^{-z^2/2}\,dz
=\frac2{\sqrt{2\pi}}\int_0^\infty z^2e^{-z^2/2}\,dz.
$$

Comparing these two [integrals](../../../../../../integral-split.md) gives

$$
\boxed{\mathbb E[X]=\sqrt{\frac\pi2}\,\mathbb E[Z^2],\qquad\beta=\sqrt{\frac\pi2}.}
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
