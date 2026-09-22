<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define $g\cdot(g_1H)=(gg_1)H$ on the set of [left cosets](../../../../../../../left-coset.md). It is well-defined: if $g_1H=g_2H$, then $g_2=g_1h$ for some $h\in H$, so $(gg_2)H=(gg_1h)H=(gg_1)H$. The identity fixes each coset, and associativity in $G$ gives

$$
g\cdot(h\cdot(g_1H))=(ghg_1)H=(gh)\cdot(g_1H).
$$

Hence this is a left [group action](../../../../../../../group-action-split.md), and part (a) supplies its [group homomorphism](../../../../../../../group-homomorphism.md) $\Phi:G\to\operatorname{Sym}(S)$.

An element of the [kernel of a group homomorphism](../../../../../../../kernel-of-a-group-homomorphism.md) $\Phi$ fixes every coset, in particular $H$ itself. Thus $g\in\ker\Phi$ implies $gH=H$, which implies $g\in H$. Therefore

$$
\boxed{\ker\Phi\leq H.}
$$

The subgroup symbol is justified because a [kernel of a group homomorphism](../../../../../../../kernel-of-a-group-homomorphism.md) is a [subgroup](../../../../../../../subgroup.md), and the argument proves containment.

## ↑ Ancestors (13)

1. [I](../i.md)
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
