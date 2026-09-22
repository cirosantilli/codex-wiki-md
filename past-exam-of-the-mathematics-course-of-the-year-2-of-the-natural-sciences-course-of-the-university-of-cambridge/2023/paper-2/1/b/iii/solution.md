<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Expand the solution and the forcing in the orthonormal [Sturm-Liouville eigenfunction expansion](../../../../../../sturm-liouville-eigenfunction-expansion.md). The forcing coefficients are

$$
b_n=\langle y_n,1\rangle_w
=\sqrt2\int_0^1\sin(n\pi t)\,dt
=\frac{\sqrt2[1-(-1)^n]}{n\pi}.
$$

Every $\lambda_n$ is nonzero, so the solution coefficient is $b_n/\lambda_n$. Thus

$$
\boxed{y(x)=\sum_{n=1}^{\infty}\frac{2[1-(-1)^n]}{n\pi(n^2\pi^2-1)}\sin(n\pi\log x)
=\sum_{\substack{n\geq1\\n\text{ odd}}}\frac{4\sin(n\pi\log x)}{n\pi(n^2\pi^2-1)}.}
$$

As an independent check, solving $Y''+Y=-1$ directly with the two endpoint conditions gives

$$
y(x)=\frac{\cos(\log x-\tfrac12)}{\cos(\tfrac12)}-1.
$$

It satisfies both [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) and the forced [ordinary differential equation](../../../../../../ordinary-differential-equation.md).

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
