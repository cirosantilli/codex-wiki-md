<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

A [normal subgroup](../../../../normal-subgroup.md) $H$ satisfies $gHg^{-1}=H$ for every $g\in G$. A [group homomorphism](../../../../group-homomorphism.md) preserves multiplication, $\Phi(ab)=\Phi(a)\Phi(b)$. It follows that $\Phi(e_1)=e_2$ and $\Phi(g^{-1})=\Phi(g)^{-1}$.

The [kernel of a group homomorphism](../../../../kernel-of-a-group-homomorphism.md) $K=\{g:\Phi(g)=e_2\}$ contains the identity and satisfies $ab^{-1}\in K$ for $a,b\in K$, so is a subgroup. For $k\in K$, $\Phi(gkg^{-1})=\Phi(g)e_2\Phi(g)^{-1}=e_2$. Thus $gKg^{-1}\subseteq K$, and applying the same inclusion to $g^{-1}$ gives equality. Hence the kernel is a [normal subgroup](../../../../normal-subgroup.md).

The product $f=\prod_{i<j}(x_i-x_j)$ is a [Vandermonde determinant](../../../../vandermonde-determinant.md) up to a fixed overall sign. A transposition exchanging $x_p,x_q$ reverses their mutual factor. Every other factor involving one of these variables is paired with the corresponding factor involving the other; those paired products are unchanged. Therefore

$$
\boxed{f\longmapsto-f\quad\text{under every transposition}.}
$$

If a permutation has decompositions into $r$ and $s$ transpositions, they act as $(-1)^rf$ and $(-1)^sf$. This polynomial is nonzero, for example at pairwise distinct real inputs, so the signs must agree. Thus **all decompositions have the same parity**, and an even decomposition forces every decomposition to be even. This defines the [sign of a permutation](../../../../sign-of-a-permutation.md); its kernel is the [alternating group](../../../../alternating-group.md), linking the parity argument to the normal-kernel result above.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 2](../../paper-2-split.md)
3. [2006](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
