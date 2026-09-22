<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First supply the unlettered preliminaries. Assuming the relevant [categorical limits](../../../../../../categorical-limit.md) and [colimits](../../../../../../colimit.md) exist, limits of shape $I$ commute with colimits of shape $J$ when for every [functor](../../../../../../functor.md) $D:I\times J\to\mathcal C$ the canonical map

$$
\boxed{\operatorname*{colim}_{j\in J}\operatorname*{lim}_{i\in I}D(i,j)
\longrightarrow\operatorname*{lim}_{i\in I}\operatorname*{colim}_{j\in J}D(i,j)}
$$

is an [isomorphism](../../../../../../isomorphism.md). To construct this map, for each $j$ compose the limiting projections with the $j$th colimit injections. They form an $I$-cone, giving a map into the right-hand [categorical limit](../../../../../../categorical-limit.md); these maps form a $J$-cocone, giving the comparison. This specifies the actual comparison required for [commutation of limits and colimits](../../../../../../commutation-of-limits-and-colimits.md).

A [group](../../../../../../group-split.md) regarded as a one-object [category](../../../../../../category-split.md) has its group elements as arrows, with composition given by multiplication. A [functor](../../../../../../functor.md) from it to the [Category of sets](../../../../../../category-of-sets.md) is a [group action](../../../../../../group-action.md). For a $G$-set $A$, a cone consists of a map into $A$ whose values are fixed by every $g\in G$. Hence its [categorical limit](../../../../../../categorical-limit.md) is the set $A^G$ of [fixed points of a group action](../../../../../../fixed-point-of-a-group-action.md). A cocone is a map out of $A$ constant on [orbits of a group action](../../../../../../orbit-of-a-group-action.md); its universal quotient is the orbit set. Thus

$$
\boxed{\lim_GA=A^G,\qquad\operatorname*{colim}_GA=A/G.}
$$

A [diagram in a category](../../../../../../diagram-category-theory.md) $G\times H\to\mathbf{Set}$ is a set $A$ with commuting [group actions](../../../../../../group-action.md) of $G$ and $H$. Its limit–colimit comparison is

$$
\theta:A^G/H\longrightarrow(A/H)^G,\qquad[a]_H\longmapsto[a]_H.
$$

Commutation makes $A^G$ stable under $H$. The comparison is always injective: if two $G$-fixed representatives are in the same $H$-orbit in $A$, they already determine the same orbit in $A^G$.

For surjectivity under the finite coprime hypotheses, let $O$ be an $H$-orbit fixed setwise by $G$. Its size divides $|H|$ by the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md). Since the [group actions](../../../../../../group-action.md) commute and $H$ is transitive on $O$, all $G$-orbits inside $O$ have the same size $d$: the bijection $a\mapsto ha$ identifies the $G$-orbits of $a$ and $ha$. Thus $d$ divides $|O|$, while the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) also gives $d\mid|G|$. The orders are [coprime](../../../../../../coprime-integers.md), so $d=1$. Every point in $O$ is therefore $G$-fixed, and $O$ lies in the image of $\theta$. We have proved [commutation of fixed points and orbit quotients for coprime groups](../../../../../../commutation-of-fixed-points-and-orbit-quotients-for-coprime-groups.md):

$$
\boxed{A^G/H\cong(A/H)^G.}
$$

The bijection is the canonical comparison and is natural in the set with commuting [group actions](../../../../../../group-action.md), so it proves the requested [commutation of limits and colimits](../../../../../../commutation-of-limits-and-colimits.md) in the [Category of sets](../../../../../../category-of-sets.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
