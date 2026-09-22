<h1 id="10g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [compact space](../../../../../../compact-space.md) is a [topological space](../../../../../../topological-space.md) in which every [open cover](../../../../../../open-cover.md) has a finite subcover. A [Hausdorff space](../../../../../../hausdorff-space.md) is one in which every two distinct points have disjoint open neighbourhoods. A [homeomorphism](../../../../../../homeomorphism.md) is a bijection that is continuous and whose inverse is continuous.

For an [equivalence relation](../../../../../../equivalence-relation.md) $R$ on $X$, let $X/R$ be the set of equivalence classes and let

$$
q:X\longrightarrow X/R,
\qquad q(x)=[x].
$$

The [quotient topology](../../../../../../quotient-topology.md) declares $U\subseteq X/R$ open exactly when $q^{-1}(U)$ is open in $X$. It follows directly from the definition that $q$ is continuous.

Suppose that the continuous map $f:X\to Y$ is constant on equivalence classes. The only possible factorisation is

$$
F:X/R\longrightarrow Y,
\qquad F([x])=f(x),
$$

which is well-defined by the hypothesis and satisfies $F\circ q=f$. For every open $V\subseteq Y$,

$$
q^{-1}(F^{-1}(V))=f^{-1}(V)
$$

is open in $X$. The definition of the quotient topology therefore makes $F^{-1}(V)$ open, so $F$ is continuous. This proves the [universal property of the quotient topology](../../../../../../universal-property-of-the-quotient-topology.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10G](../../10g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
