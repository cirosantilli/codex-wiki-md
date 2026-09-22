<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

A [subgroup](../../../../../subgroup.md) $K$ is a [normal subgroup](../../../../../normal-subgroup.md) of $G$ when $gKg^{-1}=K$ for every $g\in G$.

For a [group homomorphism](../../../../../group-homomorphism.md) $\phi:G\to H$, its kernel contains the identity and, for $x,y$ in the kernel, $\phi(xy^{-1})=\phi(x)\phi(y)^{-1}=e$. Hence the [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is a [subgroup](../../../../../subgroup.md). Also $\phi(gkg^{-1})=\phi(g)e\phi(g)^{-1}=e$ for $k$ in the kernel; applying this to $g$ and $g^{-1}$ gives equality under conjugation. Thus **the kernel is always normal**.

The image contains the identity and is closed under products and inverses, so the [image of a group homomorphism](../../../../../image-of-a-group-homomorphism.md) is always a [subgroup](../../../../../subgroup.md) of the target. It need not be normal: include $C_2=\{e,(12)\}$ into $S_3$. Conjugation by $(123)$ takes $(12)$ to $(23)$, outside that image. Thus **the image is not always normal**.

For matrices over either $\mathbb Z$ or $\mathbb F_2=\mathbb Z_2$, multiplication stays in the same coefficient ring, and [determinants](../../../../../determinant.md) multiply, so the determinant-one matrices are closed. Associativity is inherited from matrix multiplication, the identity has [determinant](../../../../../determinant.md) one, and the inverse is

$$
\boxed{\begin{pmatrix}a&b\\c&d\end{pmatrix}^{-1}
=\begin{pmatrix}d&-b\\-c&a\end{pmatrix}\quad(ad-bc=1).}
$$

Its entries are still in the same ring and its [determinant](../../../../../determinant.md) is one. This proves that both sets are [special linear groups](../../../../../special-linear-group.md) under multiplication. Over $\mathbb F_2$, minus and plus agree, and the same formula applies.

Reduction of integers modulo two preserves addition and multiplication. Therefore reducing entries preserves the [determinant](../../../../../determinant.md) condition and satisfies $\phi(AB)=\phi(A)\phi(B)$, proving the stated map is a [group homomorphism](../../../../../group-homomorphism.md).

Its target acts on the three nonzero vectors of $\mathbb F_2^2$. The action is faithful: a matrix fixing all three vectors fixes the two standard basis vectors and so is the identity. Thus its image, and in particular the image of $\phi$, is isomorphic to a [permutation](../../../../../permutation.md) [subgroup](../../../../../subgroup.md) of $S_3$. In fact [SL2 over F2 as a permutation group](../../../../../sl2-over-f2-as-a-permutation-group.md) identifies the entire image. There are $3$ choices for the first nonzero column and $2$ for a second independent column, hence six invertible matrices. Every invertible matrix has [determinant](../../../../../determinant.md) one over $\mathbb F_2$, so the faithful action is onto $S_3$.

To show the integer reduction map reaches all of them, take

$$
S=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
T=\begin{pmatrix}1&1\\0&1\end{pmatrix}\quad\text{in }\mathrm{SL}_2(\mathbb Z).
$$

On $\{e_1,e_2,e_1+e_2\}$, the reduction of $S$ exchanges $e_1,e_2$ and fixes their sum, while the reduction of $T$ fixes $e_1$ and exchanges the other two. These two transpositions generate $S_3$. Hence

$$
\boxed{\operatorname{im}\phi=\mathrm{SL}_2(\mathbb F_2)\cong S_3.}
$$

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
