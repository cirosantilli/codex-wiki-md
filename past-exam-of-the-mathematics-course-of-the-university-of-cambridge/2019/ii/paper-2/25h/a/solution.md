<h1 id="25h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $T=\alpha'(s)$. Since $s$ is [arc length](../../../../../../arc-length.md), $|T|=1$, so $T'\perp T$. The [curvature of a space curve](../../../../../../curvature-of-a-space-curve.md) is

$$
k(s)=|T'(s)|=|\alpha''(s)|.
$$

Where $k(s)\ne0$, define the principal normal and binormal by

$$
N=\frac{T'}k,
\qquad
B=T\times N,
$$

and define the [torsion of a space curve](../../../../../../torsion-of-a-curve.md) by

$$
\tau=-B'\cdot N.
$$

Thus torsion requires nonzero curvature, so that $N$ and $B$ are defined.

Differentiating the orthonormality relations for the frame $(T,N,B)$ shows that its derivative matrix is skew-symmetric. Since $T'=kN$, differentiating $B=T\times N$ and using the definition of $\tau$ gives the [Frenet-Serret formulas](../../../../../../frenet-serret-formulas.md)

$$
\boxed{
T'=kN,
\qquad
N'=-kT+\tau B,
\qquad
B'=-\tau N.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25H](../../25h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
