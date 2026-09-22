<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

For the [centralizer of a subset](../../../../../centralizer-of-a-subset.md), the identity commutes with every $h\in A$. If $g,k$ commute with each member of $A$, then for every such $h$,

$$
(gk)h=g(kh)=g(hk)=(gh)k=h(gk).
$$

Also $gh=hg$ implies $g^{-1}h=hg^{-1}$ after multiplication by $g^{-1}$ on both sides. Thus identity, products and inverses lie in $C(A)$, proving that it is a [subgroup](../../../../../subgroup.md).

For the [conjugation action](../../../../../conjugation-action.md), identity acts trivially, and

$$
\rho(g_1,\rho(g_2,h))=g_1g_2h g_2^{-1}g_1^{-1}
=\rho(g_1g_2,h).
$$

These are the defining laws of a left [group action](../../../../../group-action.md). Its [orbits of a group action](../../../../../orbit-of-a-group-action.md) are the [conjugacy classes](../../../../../conjugacy-class.md). The stabilizer of $h$ is exactly its [centralizer](../../../../../centralizer.md), since $ghg^{-1}=h$ if and only if $gh=hg$. The [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) therefore gives

$$
|O_i|=[G:C(\{h_i\})]=\frac{|G|}{|C(\{h_i\})|}.
$$

A class has one element exactly when that element commutes with all of $G$, so the singleton classes are precisely the elements of $C(G)$, the [centre of a group](../../../../../center-of-a-group.md). Partitioning $G$ into all its [conjugacy classes](../../../../../conjugacy-class.md) now proves the [class equation](../../../../../class-equation.md)

$$
\boxed{|G|=|C(G)|+\sum_{|O_i|>1}\frac{|G|}{|C(\{h_i\})|}}.
$$

For $|G|=p^r$, [Lagrange's theorem for finite groups](../../../../../lagrange-s-theorem.md) makes every class size a power of $p$. A nonsingleton class has size at least $p$ and is therefore divisible by $p$. Reducing the [class equation](../../../../../class-equation.md) modulo $p$ yields $|C(G)|\equiv0\pmod p$, because $r>0$. The identity lies in $C(G)$, so its order is positive and divisible by $p$. Consequently

$$
\boxed{|C(G)|\ge p>1}.
$$

This proves the [nontrivial center of a finite p-group](../../../../../nontrivial-center-of-a-finite-p-group.md) directly from the conjugation classes.

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
