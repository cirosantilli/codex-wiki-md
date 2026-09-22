<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a finite [acyclic quiver](../../../../../acyclic-quiver.md), the [arrow ideal of a path algebra](../../../../../arrow-ideal-of-a-path-algebra.md) $R$ is nilpotent, and $A/R\cong\prod_{i\in Q_0}k$. If $S$ is a [simple module](../../../../../irreducible-module.md), its [submodule](../../../../../submodule.md) $RS$ is either zero or $S$. The latter would imply $R^dS=S$ for every $d$, contradicting nilpotence. Thus $RS=0$, and a simple module over the product of fields is supported at one coordinate. Therefore **the simples are exactly $S(i)$**, with $k$ at $i$, zero elsewhere, and zero arrows; the vertex $i$ is unique.

A finite-dimensional [semisimple module](../../../../../semisimple-module.md) is consequently $\bigoplus_iS(i)^{\oplus n_i}$, where $n_i=\dim X_i$. Its [dimension vector of a quiver representation](../../../../../dimension-vector-of-a-quiver-representation.md) determines its isomorphism class.

For an arbitrary finite quiver, cycles allowed, the [vertex projective module of a path algebra](../../../../../vertex-projective-module-of-a-path-algebra.md) is $P(i)=Ae_i$. Its space at vertex $j$ has [basis](../../../../../basis.md) all paths from $i$ to $j$, and an arrow acts by adjoining that arrow at the end of the path. Its [endomorphism ring](../../../../../endomorphism-ring.md) is

$$
\boxed{\operatorname{End}_A(P(i))\cong(e_iAe_i)^{\mathrm{op}}},
$$

where $e_iAe_i$ is spanned by the closed paths based at $i$. The opposite multiplication appears because endomorphisms act by right multiplication.

The [evaluation isomorphism for a vertex projective](../../../../../evaluation-isomorphism-for-a-vertex-projective.md) is

$$
\boxed{\operatorname{Hom}_Q(P(i),X)\longrightarrow X_i,\qquad h\longmapsto h(e_i)}.
$$

For $x\in X_i$, its inverse sends a path $p$ starting at $i$ to $px$. This proves both injectivity and surjectivity, and is natural in $X$. Vertex evaluation is exact, so $P(i)$ is a [projective module](../../../../../projective-module.md); alternatively it is a direct summand of the free module $A$.

The [closed-path corner of a path algebra is a domain](../../../../../closed-path-corner-of-a-path-algebra-is-a-domain.md): in a product of two nonzero linear combinations, choose their longest path lengths. Concatenation in that top degree has a unique cut at those lengths, so a product of two nonzero top coefficients cannot cancel. Hence its only [idempotents](../../../../../idempotent.md) are zero and one. The same is true of the opposite ring, proving $P(i)$ is an [indecomposable module](../../../../../indecomposable-module.md), even when cycles make it infinite-dimensional.

For $1\to2\leftarrow3$, the paths starting at vertex $1$ are $e_1$ and the arrow $1\to2$. Thus the displayed $k\xrightarrow{1}k\leftarrow0$ is **$P(1)$ and is projective**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
