<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Since $S^\mu\subset M^\mu$, Question 2 shows that every [composition factor](../../../../../composition-factor.md) of $S^\mu$ is $D^\lambda$ for a [regular partition](../../../../../regular-partition.md) $\lambda\unrhd\mu$. If $\mu$ is regular, its radical quotient $D^\mu$ occurs once: it occurs as a quotient, and its multiplicity is bounded above by the multiplicity one in $M^\mu$. All remaining factors have strictly dominating labels. A nonregular row has only strictly dominating regular labels.

Define $d_{\mu\lambda}=[S^\mu:D^\lambda]$. Order the row labels, all [partitions of an integer](../../../../../partition-of-an-integer.md) of $n$, and the column labels, the regular [partitions of an integer](../../../../../partition-of-an-integer.md), by the same total order refining decreasing dominance. Then

$$
\boxed{d_{\mu\lambda}=0\text{ unless }\lambda\unrhd\mu,
\qquad d_{\lambda\lambda}=1.}
$$

The matrix is generally rectangular. Its submatrix on regular rows is lower unitriangular in this decreasing convention; placing least dominant shapes first would transpose the visual triangular convention, not the indices.

This is the [decomposition matrix](../../../../../decomposition-matrix-modular-representation-theory.md), not just an abstract [composition factor](../../../../../composition-factor.md) table. The [standard polytabloid basis](../../../../../standard-polytabloid-basis.md) makes $S^\mu_{\mathbb Z}$ a free invariant integral lattice whose extension to [characteristic zero](../../../../../characteristic-zero.md) is the ordinary [irreducible](../../../../../irreducible-representation.md) $S^\mu$. Reducing this same lattice modulo $p$ gives exactly the modular $S^\mu$. On [p-regular elements](../../../../../p-regular-element.md), reduction of its ordinary [character](../../../../../character-of-a-representation.md) is the sum of the [Brauer characters](../../../../../brauer-character.md) of its [composition factors](../../../../../composition-factor.md), with coefficients $d_{\mu\lambda}$. These are the defining decomposition numbers; the resulting class in the [modular representation ring](../../../../../modular-representation-ring.md) is independent of the chosen invariant lattice.

For $S_3$, take rows $(3),(2,1),(1,1,1)$ in that order. In [characteristic zero](../../../../../characteristic-zero.md), or $p>3$, all three [Specht modules](../../../../../specht-module.md) are [irreducible](../../../../../irreducible-representation.md) by [Maschke's theorem](../../../../../maschke-s-theorem.md), and

$$
\boxed{M=I_3.}
$$

For $p=2$ the regular labels are $(3),(2,1)$ and

$$
\boxed{M=\begin{pmatrix}1&0\\0&1\\1&0\end{pmatrix}.}
$$

Indeed the [sign representation](../../../../../sign-representation.md) equals the [trivial representation](../../../../../trivial-representation.md). The two-dimensional $S^{(2,1)}$ is the sum-zero subspace of the three-point [permutation module](../../../../../permutation-module.md). Over an algebraic closure, a $3$-cycle has two distinct nontrivial third-root [eigenvalues](../../../../../eigenvalue.md) there, and a [transposition](../../../../../transposition-permutation.md) exchanges their lines. Neither line is invariant under $S_3$, proving [absolute irreducibility](../../../../../absolute-irreducibility-of-a-group-representation.md).

For $p=3$ the regular labels are $(3),(2,1)$ and

$$
\boxed{M=\begin{pmatrix}1&0\\1&1\\0&1\end{pmatrix}.}
$$

In the same sum-zero space the vector $(1,1,1)$ now spans an invariant trivial line. Its one-dimensional quotient is sign: the [determinant](../../../../../determinant.md) of the sum-zero representation is sign, and the [determinant](../../../../../determinant.md) of the invariant line is trivial. Therefore $S^{(2,1)}$ has one trivial and one sign factor, with sign its simple [head](../../../../../head-of-a-module.md) $D^{(2,1)}$. The bottom [Specht module](../../../../../specht-module.md) is itself sign. This proves every entry of the three possible matrices.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
