<h1 id="1/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In logarithmic coordinates the [eigenvalue problem](../../../../../../eigenvalue-problem.md) becomes $-Y''=(\lambda+1)Y$. A nonzero function with zero values at both ends requires $\lambda+1>0$: multiplying by $Y^*$ and integrating gives $(\lambda+1)\int_0^1|Y|^2dt=\int_0^1|Y'|^2dt>0$. Write $\kappa=\sqrt{\lambda+1}$. The first endpoint gives $Y=A\sin\kappa t$, and the second requires $\kappa=n\pi$, $n=1,2,\ldots$.

For [vector normalization](../../../../../../vector-normalization.md), $\int_1^e|y|^2dx/x=|A|^2\int_0^1\sin^2(n\pi t)dt=|A|^2/2$. A positive real normalization constant therefore gives

$$
\boxed{\lambda_n=n^2\pi^2-1,\qquad y_n(x)=\sqrt2\sin(n\pi\ln x),\quad n\geq1.}
$$

The sine [orthogonality](../../../../../../orthogonal-vectors.md) identity also gives $\int_1^ey_m y_n\,dx/x=\delta_{mn}$. Completeness is the usual completeness of the [Fourier sine series](../../../../../../fourier-sine-series.md) on $(0,1)$ under the logarithmic coordinate transformation.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
