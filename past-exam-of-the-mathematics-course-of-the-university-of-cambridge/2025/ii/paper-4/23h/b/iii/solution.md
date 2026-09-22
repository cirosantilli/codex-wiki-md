<h1 id="23h/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose $\phi\in C_c^\infty(\mathbb R)$ with $\lVert\phi\rVert_2=1$, and for $R>0$ set

$$
u_R(x)=R^{-1/2}\phi(x/R).
$$

A change of variables gives

$$
\lVert u_R\rVert_2=1,
\qquad
\int_\mathbb R|u_R'(x)|^2\,dx
=R^{-2}\int_\mathbb R|\phi'(x)|^2\,dx.
$$

The latter tends to zero as $R\to\infty$. Since the energy is nonnegative,

$$
\boxed{
\inf_{\substack{u\in H^1(\mathbb R)\\\lVert u\rVert_2=1}}
\int_\mathbb R|u'(x)|^2\,dx=0.
}
$$

This is [vanishing Dirichlet energy by dilation on the line](../../../../../../../vanishing-dirichlet-energy-by-dilation-on-the-line.md).

The infimum is not attained. If an admissible $u$ had zero energy, then its weak derivative would vanish almost everywhere, so $u$ would be constant almost everywhere. The only constant in $L^2(\mathbb R)$ is zero, contradicting $\lVert u\rVert_2=1$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [23H](../../../23h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
