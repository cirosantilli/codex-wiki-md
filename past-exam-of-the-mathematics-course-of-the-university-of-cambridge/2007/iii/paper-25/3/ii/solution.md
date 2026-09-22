<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each $d\in\mathcal D$, let $P(d)=\pi_0(d\downarrow F)$, the collection of connected components, where connectedness means connection by a zigzag of arrows. Precomposition with $u:d\to d'$ gives a function $P(u):P(d')\to P(d)$. Identity and composition are inherited from precomposition.

Construct a [category](../../../../../../category-split.md) $\mathcal E$ whose objects are pairs $(d,c)$ with $c\in P(d)$. An arrow $(d,c)\to(d',c')$ is an arrow $u:d\to d'$ satisfying $c=P(u)c'$. Composition is that of $\mathcal D$, and the component equation is preserved by composition. The projection $p:\mathcal E\to\mathcal D$ is a [discrete fibration](../../../../../../discrete-fibration.md): an arrow $u:d\to d'$ has precisely one lift into $(d',c')$, namely the arrow from $(d,P(u)c')$ represented by $u$.

Define $J:\mathcal C\to\mathcal E$ by

$$
J(a)=(Fa,[(a,1_{Fa})]),\qquad J(j)=F(j).
$$

This is well defined because $(a,1_{Fa})$ and $(a',Fj)$ lie in the same component of $(Fa\downarrow F)$ whenever $j:a\to a'$. Clearly $pJ=F$.

For an object $(d,c)$ of $\mathcal E$, an object of $((d,c)\downarrow J)$ is exactly a pair $(a,u:d\to Fa)$ representing the component $c$. Its morphisms are exactly the arrows in $(d\downarrow F)$ between such objects. Thus this [comma category](../../../../../../comma-category.md) is the component $c$ itself, which is nonempty and connected. This proves that $J$ is a [final functor](../../../../../../final-functor.md), and hence

$$
\boxed{F=pJ,\qquad J\text{ final},\quad p\text{ a discrete fibration}.}
$$

This is the [final-discrete-fibration factorization](../../../../../../final-discrete-fibration-factorization.md). For small [categories](../../../../../../category-split.md) the collections $P(d)$ are sets and this construction is the [category of elements](../../../../../../category-of-elements.md) of the presheaf $P$. For [categories](../../../../../../category-split.md) of a larger size, the construction is interpreted in the same chosen ambient size framework.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
