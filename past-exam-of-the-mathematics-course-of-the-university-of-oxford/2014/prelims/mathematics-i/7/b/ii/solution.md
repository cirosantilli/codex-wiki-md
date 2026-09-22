<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By [Lagrange's theorem](../../../../../../../lagrange-s-theorem.md), the [index of a subgroup](../../../../../../../index-of-a-subgroup.md) is $[G:H]=75/25=3$. Thus the set of [left cosets](../../../../../../../left-coset.md) has three elements, and the preceding [group action](../../../../../../../group-action-split.md) yields a [group homomorphism](../../../../../../../group-homomorphism.md) $\Phi:G\to S_3$ after labelling them.

Its image is a [subgroup](../../../../../../../subgroup.md) of $S_3$, so its order divides $6$. By the [first isomorphism theorem](../../../../../../../first-isomorphism-theorem.md), $|\operatorname{im}\Phi|=|G|/|\ker\Phi|$ also divides $75$. Hence its order divides $\gcd(6,75)=3$, giving possibilities $1$ and $3$. The action on cosets is [transitive](../../../../../../../transitive-relation.md): $g_2g_1^{-1}$ sends $g_1H$ to $g_2H$. It cannot be the trivial action on a three-element set, so the image does not have order $1$. Therefore

$$
\boxed{|\operatorname{im}\Phi|=3.}
$$

It follows that $|\ker\Phi|=75/3=25$. Part (b)(i) gives $\ker\Phi\leq H$, and $|H|=25$; equal finite orders force equality. A [kernel of a group homomorphism](../../../../../../../kernel-of-a-group-homomorphism.md) is a [normal subgroup](../../../../../../../normal-subgroup.md), so

$$
\boxed{H=\ker\Phi\mathrel{\trianglelefteq}G.}
$$

This is an instance of the fact that a [subgroup of index the smallest prime divisor is normal](../../../../../../../subgroup-of-index-the-smallest-prime-divisor-is-normal.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
