<h1 id="26g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\gamma$ be a $C^3$ [regular curve](../../../../../../regular-curve.md) parametrized by [arc length](../../../../../../arc-length.md), so $|\gamma'(s)|=1$. Define the [Frenet frame](../../../../../../frenet-frame.md)

$$
T=\gamma',
\qquad
\kappa=|T'|,
\qquad
N=\frac{T'}{\kappa},
\qquad
B=T\times N,
$$

and define the torsion by

$$
\tau=-B'\mathbin\cdot N.
$$

Thus curvature requires two derivatives, while $N,B,$ and torsion require $\kappa>0$; the displayed classical torsion requires three derivatives. At a point where $\kappa=0$, $N,B,$ and $\tau$ are not defined by this construction.

Since $(T,N,B)$ is an orthonormal frame, differentiating its inner products shows that its derivative matrix is skew-symmetric. The definition gives $T'=\kappa N$. Next,

$$
N'\mathbin\cdot T=-N\mathbin\cdot T'=-\kappa,
\qquad
N'\mathbin\cdot N=0,
$$

so $N'=-\kappa T+cB$. As $B'=T\times N'$ and $T\times B=-N$, we have $B'=-cN$; hence $c=-B'\cdot N=\tau$. The [Frenet-Serret formulas](../../../../../../frenet-serret-formulas.md) are therefore

$$
\boxed{
T'=\kappa N,
\qquad
N'=-\kappa T+\tau B,
\qquad
B'=-\tau N.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26G](../../26g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
