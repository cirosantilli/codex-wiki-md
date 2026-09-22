<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [tautological bundle](../../../../../../tautological-bundle.md) $\mathcal O(-1)$ over [Complex projective space](../../../../../../complex-projective-space.md) has fibre over $[\ell]$ equal to the line $\ell\subset\mathbb C^{r+1}$. Define $\mathcal O(1)=\mathcal O(-1)^*$ and the [twisting sheaf on projective space](../../../../../../twisting-sheaf-on-projective-space.md), viewed analytically as a [holomorphic line bundle](../../../../../../holomorphic-line-bundle.md), by

$$
\mathcal O(d)=
\begin{cases}\mathcal O(1)^{\otimes d},&d>0,\\
\mathcal O,&d=0,\\
\mathcal O(-1)^{\otimes(-d)},&d<0.
\end{cases}
$$

For $\mathbb{CP}^1$, use coordinates $z=Z_1/Z_0$ and $w=Z_0/Z_1=1/z$. The tautological frames $(1,z)$ and $(w,1)$ differ by $z^{-1}$, so frames $e_0,e_1$ for $\mathcal O(d)$ satisfy $e_1=z^d e_0$. A global [holomorphic section](../../../../../../holomorphic-section.md) is therefore described by entire functions $s_0(z),s_1(w)$ with

$$
s_1(w)=w^d s_0(1/w).
$$

Write $s_0(z)=\sum_{k\geq0}a_kz^k$. Holomorphicity of $s_1$ at zero permits only the powers $w^{d-k}$ with $d-k\geq0$. For $d\geq0$, this says $s_0$ is a [polynomial](../../../../../../polynomial-split.md) of degree at most $d$; for $d<0$, every coefficient must vanish. Equivalently, when $d\geq0$ the sections are [homogeneous polynomials](../../../../../../homogeneous-polynomial.md) of degree $d$ in $Z_0,Z_1$. Thus

$$
\boxed{\dim_{\mathbb C}H^0(\mathbb{CP}^1,\mathcal O(d))=
\begin{cases}d+1,&d\geq0,\\0,&d<0.\end{cases}}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
