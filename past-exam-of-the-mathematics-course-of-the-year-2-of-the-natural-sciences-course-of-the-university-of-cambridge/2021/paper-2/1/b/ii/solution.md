<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $z=x^3/3$ and write $y(x)=Y(z)$. Then

$$
y'=x^2Y_z,\qquad y''=2xY_z+x^4Y_{zz},
$$

so the two first-derivative contributions cancel exactly, leaving

$$
-Y_{zz}-aY=\lambda Y,\qquad Y(0)=Y(1/3)=0.
$$

The Dirichlet spectrum of $-d^2/dz^2$ on this interval is $(3n\pi)^2$, $n\geq1$. If $\lambda+a\leq0$, the linear or hyperbolic solutions cannot satisfy both zero endpoints nontrivially, so no additional modes have been omitted. Thus

$$
\boxed{\lambda_n=9n^2\pi^2-a,\qquad y_n(x)=\sqrt6\sin(n\pi x^3),\qquad n=1,2,\ldots.}
$$

To verify normalization, use $dz=x^2dx$:

$$
\int_0^1x^2\sin(n\pi x^3)\sin(m\pi x^3)dx=\int_0^{1/3}\sin(3n\pi z)\sin(3m\pi z)dz=\frac{\delta_{nm}}6.
$$

This proves weighted orthonormality and also transfers completeness from the ordinary [Fourier sine series](../../../../../../fourier-sine-series.md). The construction is the [cubic-coordinate reduction of a singular Sturm-Liouville operator](../../../../../../cubic-coordinate-reduction-of-a-singular-sturm-liouville-operator.md). The positive constant $a$ shifts the entire spectrum down; a zero [eigenvalue](../../../../../../eigenvalue.md) occurs if $a=9n^2\pi^2$, so the no-zero-eigenvalue proviso in part (a)(iii) must be imposed separately if that inverse formula is used here.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
