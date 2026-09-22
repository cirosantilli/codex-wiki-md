<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $W_j=V_{j+1}\cap V_j^\perp$, the detail space of the [multiresolution analysis](../../../../../../multiresolution-analysis.md). The [Meyer-Mallat theorem](../../../../../../meyer-mallat-theorem.md) gives a function $\psi\in W_0$ whose integer translates form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $W_0$. Dilations then give an [orthonormal basis](../../../../../../orthonormal-basis.md) of each $W_j$, and the density and trivial-intersection axioms imply

$$
\boxed{L^2(\mathbb R)=\mathop{\bigoplus}_{j\in\mathbb Z}W_j.}
$$

For an explicit filter construction, write the [scaling refinement equation](../../../../../../scaling-refinement-equation.md) $\varphi(x)=\sqrt2\sum_kh_k\varphi(2x-k)$. With a [quadrature mirror filter](../../../../../../quadrature-mirror-filter.md) one may take $g_k=(-1)^k\overline{h_{1-k}}$ and $\psi(x)=\sqrt2\sum_kg_k\varphi(2x-k)$. A harmless constant sign or integer translation gives an equivalent [orthonormal wavelet](../../../../../../orthonormal-wavelet.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
