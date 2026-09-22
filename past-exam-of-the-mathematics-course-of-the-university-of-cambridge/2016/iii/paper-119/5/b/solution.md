<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $q:G\twoheadrightarrow K$ and $r:H\twoheadrightarrow K$ be the two quotient homomorphisms. On the underlying set $A=K$, define the commuting [group actions](../../../../../../group-action.md)

$$
g\cdot k=q(g)k,\qquad h\cdot k=kr(h)^{-1}.
$$

The inverse is essential for the right multiplication formula to define a left [group action](../../../../../../group-action.md): $h_1\cdot(h_2\cdot k)=k r(h_2)^{-1}r(h_1)^{-1}=(h_1h_2)\cdot k$. Left and right multiplication commute.

Because $q$ is onto and $K$ is nontrivial, there is no [fixed point of a group action](../../../../../../fixed-point-of-a-group-action.md) for $G$: if every $q(g)k=k$, cancellation would make every element of $K$ the identity. Thus $A^G=\varnothing$. Because $r$ is onto, the $H$-action is transitive and $A/H$ is a singleton. The induced $G$-action on that singleton is trivial. Consequently the comparison is

$$
\boxed{A^G/H=\varnothing\longrightarrow(A/H)^G=\{*\},}
$$

which is not an [isomorphism](../../../../../../isomorphism.md). This proves the [common quotient obstruction to commutation of fixed points and orbits](../../../../../../common-quotient-obstruction-to-commutation-of-fixed-points-and-orbits.md), so limits of shape $G$ do not commute with colimits of shape $H$ in the [Category of sets](../../../../../../category-of-sets.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
