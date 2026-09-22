<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

Every [permutation](../../../../../permutation.md) is a product of [transpositions](../../../../../transposition-permutation.md), since a cycle can be written

$$
(a_1\,a_2\,\ldots\,a_k)=(a_1\,a_k)\cdots(a_1\,a_2)
$$

with rightmost factors acting first. Define the [sign of a permutation](../../../../../sign-of-a-permutation.md) to be $(-1)^r$ for a product of $r$ [transpositions](../../../../../transposition-permutation.md). To prove that it is well defined without assuming parity, let $P_\sigma$ be the [permutation matrix](../../../../../permutation-matrix.md) specified by $P_\sigma e_i=e_{\sigma(i)}$. Then $P_{\sigma\tau}=P_\sigma P_\tau$, and a [transposition](../../../../../transposition-permutation.md) exchanges two columns of the identity, so its [determinant](../../../../../determinant.md) is $-1$. Any decomposition into $r$ [transpositions](../../../../../transposition-permutation.md) therefore has

$$
\det P_\sigma=(-1)^r.
$$

The left-hand side depends only on $\sigma$, proving well-definedness. Multiplicativity of the [determinant](../../../../../determinant.md) now gives the [sign homomorphism](../../../../../sign-homomorphism.md):

$$
\boxed{\operatorname{sgn}(\sigma\tau)=\operatorname{sgn}(\sigma)\operatorname{sgn}(\tau).}
$$

For the first requested [group embedding](../../../../../group-embedding.md), use the [faithful four-point action of GL2 over F2](../../../../../faithful-four-point-action-of-gl2-over-f2.md): label the four [vectors](../../../../../vector.md) in $\mathbb F_2^2$ and let an invertible $2\times2$ [matrix](../../../../../matrix.md) act on them by multiplication. Composition of these actions gives a [group homomorphism](../../../../../group-homomorphism.md) $\psi:GL_2(\mathbb F_2)\to S_4$. If a matrix fixes every vector, it fixes both standard basis vectors and is the identity, so the action is faithful. The matrix

$$
B=\begin{pmatrix}0&1\\1&0\end{pmatrix}
$$

fixes $(0,0)$ and $(1,1)$ and exchanges $(1,0)$ with $(0,1)$. Its image is a single [transposition](../../../../../transposition-permutation.md), hence $\operatorname{sgn}(\psi(B))=-1$. **The composite sign map is nontrivial.**

For the second [group embedding](../../../../../group-embedding.md), simply take

$$
\boxed{\phi(\sigma)=P_\sigma\in GL_n(\mathbb R),\qquad\det\phi(\sigma)=\operatorname{sgn}(\sigma).}
$$

The preceding multiplication formula proves the [group homomorphism](../../../../../group-homomorphism.md) property, and $P_\sigma=I$ forces $\sigma(i)=i$ for every $i$, proving injectivity.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
