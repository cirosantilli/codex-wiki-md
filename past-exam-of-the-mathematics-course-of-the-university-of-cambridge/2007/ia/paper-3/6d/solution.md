<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

A [subgroup](../../../../../subgroup.md) $H$ is a [normal subgroup](../../../../../normal-subgroup.md) of $G$ if $gHg^{-1}=H$ for every $g\in G$, equivalently if $gH=Hg$ for every $g$. In the [symmetric group](../../../../../symmetric-group.md) $S_3$, the [subgroup](../../../../../subgroup.md) $A_3=\{e,(123),(132)\}$ is normal: conjugation relabels a three-cycle as a three-cycle, so preserves this set. By contrast, $\{e,(12)\}$ is not normal because conjugating $(12)$ by $(23)$ gives $(13)$ outside the [subgroup](../../../../../subgroup.md).

If $H$ is normal, define a product on its left [cosets](../../../../../coset.md) by $(gH)(kH)=(gk)H$. To check that this [quotient group](../../../../../quotient-group.md) operation is well-defined, take different representatives $gh_1$ and $kh_2$, with $h_1,h_2\in H$. Their product is

$$
gh_1kh_2=gk(k^{-1}h_1k)h_2.
$$

Normality puts the last two factors in $H$, so its [coset](../../../../../coset.md) is exactly $gkH$. Associativity follows from that in $G$, the identity [coset](../../../../../coset.md) is $H$, and the inverse of $gH$ is $g^{-1}H$. Thus all the group axioms hold, and the projection $g\mapsto gH$ is a [group homomorphism](../../../../../group-homomorphism.md).

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
