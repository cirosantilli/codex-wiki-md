<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $a$ and $b$ be the pullbacks of the standard generator of $H^n(S^n;\mathbb Z)$ from the two factors. The [Künneth theorem](../../../../../../kunneth-theorem.md) and graded commutativity of the [cup product](../../../../../../cup-product.md) give

$$
\boxed{H^*(S^n\times S^n;\mathbb Z)
=\mathbb Z\langle1,a,b,ab\rangle,qquad
|a|=|b|=n,quad a^2=b^2=0,quad ba=(-1)^n ab.}
$$

Each homeomorphism acts invertibly on $H^n\cong\mathbb Z^2$. To respect ordinary composition, send $h$ to $(h^{-1})^*$; functoriality of [induced map on cohomology](../../../../../../induced-map-on-cohomology.md) then defines a homomorphism

$$
\operatorname{Homeo}(S^n\times S^n)\longrightarrow GL(2,\mathbb Z).
$$

For $n=1$, the space is the [torus](../../../../../../torus.md). Every matrix in $GL(2,\mathbb Z)$ induces a linear homeomorphism $\mathbb R^2/\mathbb Z^2\to\mathbb R^2/\mathbb Z^2$, so the image is all of $GL(2,\mathbb Z)$.

For $n=2$, write $h^*a=pa+qb$. Since $a^2=0$ and $ab=ba$,

$$
0=(h^*a)^2=2pq,ab,
$$

so $pq=0$; the same argument applies to $h^*b$. Invertibility then forces the matrix to be a [signed permutation matrix](../../../../../../signed-permutation-matrix.md). Every such matrix is realized by swapping the two sphere factors and applying an orientation-reversing homeomorphism to either factor. Thus the image consists exactly of the eight signed permutation matrices.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
