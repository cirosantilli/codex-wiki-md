<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On a positively oriented contour encircling $z_0$ once inside an annulus of analyticity, the [Laurent series](../../../../../laurent-series.md) coefficients are

$$
\boxed{a_n=\frac1{2\pi i}\oint_C\frac{f(z)}{(z-z_0)^{n+1}}dz,\qquad n\in\mathbb Z.}
$$

This follows by inserting the convergent Laurent expansion and integrating term by term: only the term with exponent $-1$ has nonzero contour integral. Uniform convergence on compact circles in the annulus justifies that step.

For the function at hand,

$$
\frac1{z(z-1)}=-\frac1z\frac1{1-z}=-\frac1z\sum_{j=0}^\infty z^j.
$$

The [geometric series](../../../../../geometric-series.md) converges for $|z|<1$, and the pole at zero excludes the centre. Thus

$$
\boxed{\frac1{z(z-1)}=-\sum_{n=-1}^\infty z^n,\qquad 0<|z|<1.}
$$

The coefficients are $a_n=-1$ for $n\geq-1$ and zero for $n<-1$. The coefficient formula gives the same result on $|z|=\rho<1$: $a_n=(2\pi i)^{-1}\oint z^{-n-2}/(z-1)\,dz$, and expansion of $(z-1)^{-1}$ selects exactly those coefficients.

The annulus is essential. For $|z|>1$, expand instead in inverse powers:

$$
\frac1{z(z-1)}=\frac1{z^2}\frac1{1-z^{-1}}=\sum_{j=0}^\infty z^{-j-2},\qquad |z|>1.
$$

These are different Laurent expansions about the same centre on the two annuli separated by the singularity at $z=1$. The series requested in the PDF is the inner one, not a global expansion.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
