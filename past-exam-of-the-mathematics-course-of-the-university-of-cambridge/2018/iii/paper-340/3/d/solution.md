<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [multiresolution analysis](../../../../../../multiresolution-analysis.md) $V_j$ and its detail spaces $W_j$, take the completed [tensor product](../../../../../../tensor-product.md) $\mathcal V_j=V_j\otimes V_j$. Since $V_{j+1}=V_j\oplus W_j$,

$$
\mathcal V_{j+1}=\mathcal V_j\oplus(W_j\otimes V_j)\oplus(V_j\otimes W_j)\oplus(W_j\otimes W_j).
$$

The three [tensor-product wavelets](../../../../../../tensor-product-wavelet.md) are

$$
\Psi^1(x,y)=\psi(x)\varphi(y),\quad
\Psi^2(x,y)=\varphi(x)\psi(y),\quad
\Psi^3(x,y)=\psi(x)\psi(y).
$$

Taking products of members of the two one-dimensional families gives an [orthonormal basis](../../../../../../orthonormal-basis.md) of each respective completed [tensor product](../../../../../../tensor-product.md). Density and the coarse-scale trivial intersection yield

$$
\boxed{\{2^j\Psi^a(2^jx-k_1,2^jy-k_2):a=1,2,3,\ j,k_1,k_2\in\mathbb Z\}}
$$

as an [orthonormal basis](../../../../../../orthonormal-basis.md) of $L^2(\mathbb R^2)$. The normalization is $2^j$ in two dimensions. On the square, tensorize the [interval-adapted wavelet basis](../../../../../../interval-adapted-wavelet-basis.md) and include the finite coarse [scaling function](../../../../../../scaling-function.md) part.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
