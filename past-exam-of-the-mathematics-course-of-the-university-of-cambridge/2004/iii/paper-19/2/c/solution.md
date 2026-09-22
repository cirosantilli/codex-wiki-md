<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Surjectivity was proved in part (b). Fix $q\in N$ and choose a normal ball $B=B_N(q,\varepsilon)$ on which $\exp_q$ is a [diffeomorphism](../../../../../../diffeomorphism.md) from the tangent ball. For each $p\in f^{-1}(q)$ define a section

$$
s_p(\exp_qv)=\exp_p\bigl((df_p)^{-1}v\bigr),\qquad |v|<\varepsilon.
$$

Completeness of $M$ guarantees that the source [Riemannian exponential map](../../../../../../exponential-map-riemannian-geometry.md) is defined. Preservation of [geodesics](../../../../../../geodesic.md) and uniqueness of their initial-value problem give $f\circ s_p=\mathrm{id}_B$. Since $df$ is invertible, differentiation of this identity shows that $s_p$ is a local [diffeomorphism](../../../../../../diffeomorphism.md); it is injective because it is a section. Its image $U_p$ is open, and $f:U_p\to B$ is a [diffeomorphism](../../../../../../diffeomorphism.md).

These images are disjoint. If $s_p(y)=s_{p'}(y)$, lift the unique radial [geodesic](../../../../../../geodesic.md) from $y$ back to $q$ starting at that common point. Both section constructions give this same lift, and uniqueness forces its endpoint to be both $p$ and $p'$. Conversely, for any $x\in f^{-1}(B)$, lift that reversed radial [geodesic](../../../../../../geodesic.md) from $f(x)$ to $q$ starting at $x$. Completeness supplies its full finite interval; its endpoint is some $p\in f^{-1}(q)$. Reversing the lift shows $x=s_p(f(x))$. Consequently

$$
\boxed{f^{-1}(B)=\coprod_{p\in f^{-1}(q)}U_p,\qquad f|_{U_p}:U_p\longrightarrow B\text{ is a diffeomorphism}.}
$$

Every point has such an evenly covered neighborhood, proving that **the complete local [isometry](../../../../../../isometry.md) is a covering**. This argument does not assume a uniform positive source injectivity radius.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
