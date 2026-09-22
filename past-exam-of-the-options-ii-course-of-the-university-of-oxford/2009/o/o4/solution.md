<h1 id="o/o4/solution">Solution</h1>

↑ **Parent:** [O4](../o4.md)

Minimizing the sum of squared residuals gives the [normal equations for linear least squares](../../../../normal-equations-for-linear-least-squares.md), $X^TX\widehat\theta=X^TY$. Full column rank makes $X^TX$ positive definite and invertible, so the unique minimizer is

$$
\boxed{\widehat\theta=AY,\qquad A=(X^TX)^{-1}X^T}.
$$

Because $\mathbb EY=X\theta$ and $\operatorname{Cov}(Y)=\sigma^2I_n$, one has $AX=I_p$ and

$$
\mathbb E\widehat\theta=\theta,\qquad
\operatorname{Cov}(\widehat\theta)=\sigma^2AA^T
=\boxed{\sigma^2(X^TX)^{-1}}.
$$

For the alternative linear estimator the corresponding general formulas are

$$
\boxed{\mathbb E(DY)=DX\theta,\qquad\operatorname{Cov}(DY)=\sigma^2DD^T}.
$$

No normality assumption on the errors is needed for these claims.

## ↑ Ancestors (12)

1. [O4](../o4.md)
2. [O](../../o.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
