<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First consider finite-dimensional [Lie algebra representations](../../../../../../lie-algebra-representation.md). The operators representing an [abelian Lie algebra](../../../../../../abelian-lie-algebra.md) commute. They have a common [eigenvector](../../../../../../eigenvector.md): take an [eigenspace](../../../../../../eigenspace.md) for the first operator of a [basis](../../../../../../basis.md) of the algebra, observe that every remaining operator preserves it, and repeat inside this nonzero space. The resulting line is an [invariant subspace](../../../../../../invariant-subspace.md), so an [irreducible representation](../../../../../../irreducible-representation.md) must be one-dimensional. Its action has the form $xv=\lambda(x)v$ for a [linear functional](../../../../../../linear-functional.md) $\lambda$. Conversely, every such functional defines a [Lie algebra representation](../../../../../../lie-algebra-representation.md), since both the [Lie brackets](../../../../../../lie-bracket.md) in the algebra and the [commutators](../../../../../../commutator.md) of its scalar operators vanish. Distinct functionals give nonisomorphic representations. Thus **the irreducibles are precisely the characters $\lambda\in\mathfrak g^*$**.

Even without a finite-dimensional assumption on the module, this conclusion for a finite-dimensional [abelian Lie algebra](../../../../../../abelian-lie-algebra.md) follows from the [Weak Hilbert Nullstellensatz](../../../../../../weak-hilbert-nullstellensatz.md): its [universal enveloping algebra](../../../../../../universal-enveloping-algebra.md) is the [polynomial](../../../../../../polynomial-split.md) algebra $\operatorname{Sym}(\mathfrak g)$. A simple module over a commutative algebra is its quotient by a [maximal ideal](../../../../../../maximal-ideal.md), and every [maximal ideal](../../../../../../maximal-ideal.md) of this [polynomial](../../../../../../polynomial-split.md) algebra over $\mathbb C$ has residue field $\mathbb C$.

**Indecomposable does not imply irreducible.** For the one-dimensional [abelian Lie algebra](../../../../../../abelian-lie-algebra.md) $\mathbb Cx$, let $x$ act on $\mathbb C^2$ by the [Nilpotent Jordan block](../../../../../../nilpotent-jordan-block.md)

$$
N=\begin{pmatrix}0&1\\0&0\end{pmatrix}.
$$

The line spanned by the first coordinate vector is an [invariant subspace](../../../../../../invariant-subspace.md), so the module is reducible. If it were a [direct sum](../../../../../../direct-sum.md) of two nonzero submodules, both would have [dimension](../../../../../../dimension-vector-space.md) one; nilpotence would force $N$ to act as zero on both, contrary to $N\ne0$. Thus it is an [indecomposable representation](../../../../../../indecomposable-representation.md).

For a finite-dimensional module $V$, put $d=\dim V$ and define its [generalized weight spaces](../../../../../../generalized-weight-space-of-a-lie-algebra-representation.md) intrinsically by

$$
V^\lambda=\{v\in V:(\rho(x)-\lambda(x)I)^d v=0\text{ for every }x\in\mathfrak g\}.
$$

To obtain the decomposition, choose a [basis](../../../../../../basis.md) $x_1,\ldots,x_r$ of $\mathfrak g$, split into [generalized eigenspaces](../../../../../../generalized-eigenspace.md) of $\rho(x_1)$, and successively split each piece by $\rho(x_2),\ldots,\rho(x_r)$. All the pieces are submodules because the acting operators commute. On one resulting piece, $\rho(x_j)$ has a unique [eigenvalue](../../../../../../eigenvalue.md) $\lambda_j$. The commuting operators can be simultaneously upper triangularized by repeating the common-eigenvector argument on quotients. Hence on this piece every $\rho(x_j)-\lambda_j I$ is strictly upper triangular. Any [linear combination](../../../../../../linear-combination.md) is also strictly upper triangular, and its $d$th power vanishes. Extending $\lambda_j$ linearly therefore identifies the piece with $V^\lambda$. Different tuples give disjoint pieces; if a component has a different tuple from $\lambda$, at least one $\rho(x_j)-\lambda(x_j)I$ is invertible there. Consequently

$$
\boxed{V=\bigoplus_{\lambda\in\mathfrak g^*}V^\lambda,}
$$

with only finitely many nonzero summands. Since the definition uses every $x$ rather than a chosen [basis](../../../../../../basis.md), this [generalized-weight decomposition for a nilpotent Lie algebra](../../../../../../generalized-weight-decomposition-for-a-nilpotent-lie-algebra.md) is canonical. Its summands need not be irreducible, as the [Jordan block](../../../../../../jordan-block.md) example already shows.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
