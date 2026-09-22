<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the standard [CW complex](../../../../../cw-complex.md) structure on the [real projective plane](../../../../../real-projective-plane.md), with one cell $e_r$ for each $r=0,1,2$. The attaching map of the two-cell winds twice around the one-cell, so the [cellular chain complex](../../../../../cellular-chain-complex.md) has $de_2=2e_1$ and $de_1=0$.

The product cells $e_{ij}=e_i\times e_j$, $0\le i,j\le2$, give nine cells, in dimensions $0,1,2,3,4$ with counts $1,2,3,2,1$. The [cellular chains of a product of finite CW complexes](../../../../../cellular-chains-of-a-product-of-finite-cw-complexes.md) have boundary $d(e_i\times e_j)=de_i\times e_j+(-1)^ie_i\times de_j$. In the ordered bases

$$
C_1=(e_{10},e_{01}),\quad C_2=(e_{20},e_{11},e_{02}),\quad C_3=(e_{21},e_{12}),\quad C_4=(e_{22}),
$$

the nonzero matrices are

$$
d_2=\begin{pmatrix}2&0&0\\0&0&2\end{pmatrix},\qquad
d_3=\begin{pmatrix}0&0\\2&-2\\0&0\end{pmatrix},\qquad
d_4=\begin{pmatrix}2\\2\end{pmatrix},\qquad d_1=0.
$$

In particular $d_2d_3=d_3d_4=0$. The degree-one [homology](../../../../../homology-split.md) is $\mathbb Z^2/2\mathbb Z^2$. The degree-two [cellular cycles](../../../../../cellular-cycle.md) are $\mathbb Ze_{11}$, and the [cellular boundaries](../../../../../cellular-boundary.md) there are $2\mathbb Ze_{11}$. The degree-three cycles are $\mathbb Z(e_{21}+e_{12})$, whose double is the boundary of $e_{22}$. Finally $d_4$ is injective. This computes the [integral homology of two real projective planes](../../../../../integral-homology-of-two-real-projective-planes.md):

$$
\boxed{H_r(\mathbb{RP}^2\times\mathbb{RP}^2;\mathbb Z)=
\begin{cases}\mathbb Z,&r=0,\\(\mathbb Z/2)^2,&r=1,\\\mathbb Z/2,&r=2,3,\\0,&\text{otherwise}.\end{cases}}
$$

The degree-three torsion is the [Tor functor](../../../../../tor-functor.md) contribution in the [Künneth theorem](../../../../../kunneth-theorem.md); it would be missed by retaining only tensor products of the two factors' homology groups.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
