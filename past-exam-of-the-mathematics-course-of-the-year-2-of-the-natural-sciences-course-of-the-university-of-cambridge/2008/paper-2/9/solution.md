<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

The [kernel of a group homomorphism](../../../../kernel-of-a-group-homomorphism.md) is $K=\{g:\theta(g)=1_H\}$. It is a [subgroup](../../../../subgroup.md), since the identity maps to the identity and $\theta(k_1k_2^{-1})=1_H$ for $k_1,k_2\in K$. Also

$$
\theta(gkg^{-1})=\theta(g)\theta(k)\theta(g)^{-1}=1_H,
$$

so $gKg^{-1}\subseteq K$. Applying the same inclusion with $g^{-1}$ gives equality, proving that $K$ is a [normal subgroup](../../../../normal-subgroup.md).

The map $gK\mapsto\theta(g)$ is well defined, multiplicative and injective, with image $\operatorname{im}\theta$. Thus the [first isomorphism theorem](../../../../first-isomorphism-theorem.md) gives

$$
\boxed{G/K\cong\operatorname{im}\theta\leq H.}
$$

The quotient is isomorphic to all of $H$ precisely when the original homomorphism is surjective.

For the [general linear group](../../../../general-linear-group.md), the [determinant](../../../../determinant.md) gives a homomorphism $\det:\operatorname{GL}(n,\mathbb R)\to\mathbb R^\times$, since $\det(AB)=\det A\det B$. Its kernel is the [special linear group](../../../../special-linear-group.md) $\operatorname{SL}(n,\mathbb R)$, so that [subgroup](../../../../subgroup.md) is normal. Every nonzero real $t$ is the determinant of $\operatorname{diag}(t,1,\ldots,1)$ for $n\geq1$, making the map surjective. Therefore

$$
\boxed{\operatorname{GL}(n,\mathbb R)/\operatorname{SL}(n,\mathbb R)\cong\mathbb R^\times,}
$$

where the operation on the right is multiplication.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 2](../../paper-2-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
