<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a [simple pole](../../../../simple-pole.md), the [residue](../../../../residue.md) is $\operatorname{Res}_{z_0}f=\lim_{z\to z_0}(z-z_0)f(z)$, the coefficient $a_{-1}$ of its [Laurent series](../../../../laurent-series.md). On an anticlockwise circle $z=z_0+Re^{it}$, integration of each Laurent term is zero except $a_{-1}/(z-z_0)$, whose integral is $2\pi i a_{-1}$. This proves the stated single-pole [residue theorem](../../../../residue-theorem.md).

For $F(z)=e^{az}/(1+e^z)$, the only pole inside the rectangle of height $2\pi$ is $z=i\pi$, with [residue](../../../../residue.md) $e^{ai\pi}/e^{i\pi}=-e^{ai\pi}$. The [residue theorem](../../../../residue-theorem.md) therefore gives $I(R)=-2\pi i e^{ai\pi}$. The upper edge is traversed from right to left and satisfies $F(x+2\pi i)=e^{2\pi ia}F(x)$, so the two horizontal contributions sum to $(1-e^{2\pi ia})\int_{-R}^R e^{ax}/(1+e^x)dx$.

On the right edge the modulus is bounded by $e^{aR}/(e^R-1)$, and on the left by $e^{-aR}/(1-e^{-R})$. Multiplying by the fixed edge length $2\pi$ shows that both contributions tend to zero because $0<a<1$. Thus

$$
(1-e^{2\pi ia})J=-2\pi i e^{\pi ia}.
$$

Using $1-e^{2\pi ia}=-2ie^{\pi ia}\sin(\pi a)$ yields

$$
\boxed{J=\frac\pi{\sin(\pi a)}.}
$$

This [rectangular contour for an exponential beta integral](../../../../rectangular-contour-for-an-exponential-beta-integral.md) also gives the ordinary beta integral after the substitution $t=e^x$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
