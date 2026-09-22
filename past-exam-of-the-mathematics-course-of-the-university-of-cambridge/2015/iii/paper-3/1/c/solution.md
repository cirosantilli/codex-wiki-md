<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Rows in the following matrix index the source, columns the target, in the order $X,Y,Z$. Solving the arrow-square equation for a [quiver representation morphism](../../../../../../quiver-representation-morphism.md) gives

$$
\boxed{\bigl(\dim_k\operatorname{Hom}_Q(U,V)\bigr)_{U,V=X,Y,Z}=\begin{pmatrix}1&0&1\\0&1&0\\0&1&1\end{pmatrix}.}
$$

In particular, the nonzero morphisms between distinct representations are **$X\to Z$ and $Z\to Y$**, each a one-dimensional family of scalar multiples of the vertexwise inclusion or projection. A map $Y\to Z$ is forced to vanish at the source by the identity arrow of $Z$; similarly a map $Z\to X$ is forced to vanish at the target. Maps between $X$ and $Y$ are zero. Each [endomorphism ring](../../../../../../endomorphism-ring.md) is $k$.

The [extension complex of quiver representations](../../../../../../extension-complex-of-quiver-representations.md) for the [one-arrow quiver](../../../../../../kronecker-quiver-with-one-arrow.md) is

$$
\operatorname{Hom}(U_1,V_1)\oplus\operatorname{Hom}(U_2,V_2)\longrightarrow\operatorname{Hom}(U_1,V_2),\qquad(h_1,h_2)\longmapsto f_Vh_1-h_2f_U.
$$

Its [cokernel](../../../../../../cokernel.md) is $\operatorname{Ext}^1_Q(U,V)$. Substitution of the three representations gives

$$
\boxed{\bigl(\dim_k\operatorname{Ext}^1_Q(U,V)\bigr)_{U,V=X,Y,Z}=\begin{pmatrix}0&0&0\\1&0&0\\0&0&0\end{pmatrix}.}
$$

Here the first argument is the quotient endpoint of a [short exact sequence](../../../../../../short-exact-sequence.md). Thus the only possible nonsplit endpoint pair is **subobject $X$, quotient $Y$**. The sequence

$$
0\longrightarrow X\longrightarrow Z\longrightarrow Y\longrightarrow0
$$

is nonsplit, since $Z$ is indecomposable. More explicitly, all extensions with these endpoints have a middle arrow $k\xrightarrow{\lambda}k$: $\lambda=0$ gives the [split short exact sequence](../../../../../../split-short-exact-sequence.md), while each $\lambda\ne0$ gives a middle representation isomorphic to $Z$. With endpoint identifications fixed the extension classes form $k$; up to endpoint automorphisms all nonzero classes give this same nonsplit sequence. There are **no other nonsplit sequences with the listed endpoints**, including equal endpoints.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
