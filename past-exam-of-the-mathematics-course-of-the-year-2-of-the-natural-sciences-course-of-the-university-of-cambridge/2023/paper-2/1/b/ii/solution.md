<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use a [logarithmic change of variable in a Sturm-Liouville problem](../../../../../../logarithmic-change-of-variable-in-a-sturm-liouville-problem.md): set $t=\log x$ and $Y(t)=y(e^t)$. The [chain rule](../../../../../../chain-rule.md) gives

$$
y'=\frac{Y'}x,\qquad y''=\frac{Y''-Y'}{x^2},\qquad \mathcal Ly=-Y''-Y.
$$

The endpoint conditions become $Y(0)=Y(1)=0$. Multiplying $-Y''=(\lambda+1)Y$ by $Y^*$ and integrating shows that $\lambda+1>0$ for a nonzero solution. Put $\mu=\sqrt{\lambda+1}$. The first endpoint selects $Y=A\sin(\mu t)$ and the second requires $\mu=n\pi$, $n\geq1$. Hence

$$
\boxed{\lambda_n=n^2\pi^2-1,\qquad y_n(x)=\sqrt2\sin(n\pi\log x),\quad n=1,2,\ldots.}
$$

These [eigenfunctions](../../../../../../eigenfunction.md) are orthonormal in the specified [weighted inner product](../../../../../../weighted-inner-product.md), because $w(x)dx=dx/x=dt$ and

$$
\int_1^e\frac{y_m(x)y_n(x)}x\,dx
=2\int_0^1\sin(m\pi t)\sin(n\pi t)\,dt=\delta_{mn}.
$$

## ↑ Ancestors (14)

1. [Ii](../ii.md)
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
