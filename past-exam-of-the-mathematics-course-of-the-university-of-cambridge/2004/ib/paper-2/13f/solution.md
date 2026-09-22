<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

Suppose $K=\ker\varphi$ for a [group homomorphism](../../../../../group-homomorphism.md) $\varphi:G\to H$. Its identity belongs to $K$, and for $k,l\in K$ we have $\varphi(kl^{-1})=1$, so it is a [subgroup](../../../../../subgroup.md). Moreover, for $g\in G$ and $k\in K$,

$$
\varphi(gkg^{-1})=\varphi(g)\varphi(k)\varphi(g)^{-1}=1.
$$

Hence $gKg^{-1}\subseteq K$; applying this also to $g^{-1}$ gives equality, so $K$ is a [normal subgroup](../../../../../normal-subgroup.md).

Conversely, if $K$ is a [normal subgroup](../../../../../normal-subgroup.md), multiplication of cosets in the [quotient group](../../../../../quotient-group.md) $G/K$ is well-defined. The map $g\mapsto gK$ is a [group homomorphism](../../../../../group-homomorphism.md) and has [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) exactly $K$. This proves both directions without requiring $\varphi$ to be injective or surjective.

For the matrix application, reduce all entries modulo $p$:

$$
\rho:SL_2(\mathbb Z)\longrightarrow SL_2(\mathbb F_p),\qquad A\longmapsto\overline A.
$$

Reduction respects [matrix multiplication](../../../../../matrix-multiplication.md) and the [determinant](../../../../../determinant.md), so this is a [group homomorphism](../../../../../group-homomorphism.md). Its [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) consists exactly of matrices congruent to the identity modulo $p$, which are the given matrices. Therefore **$K=\ker\rho$ is a [normal subgroup](../../../../../normal-subgroup.md)**, the level-$p$ [principal congruence subgroup](../../../../../principal-congruence-subgroup.md). Surjectivity of reduction is not needed for this argument.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
