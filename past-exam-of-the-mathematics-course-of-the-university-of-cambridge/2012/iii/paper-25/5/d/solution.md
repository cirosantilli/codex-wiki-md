<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If $G$ is a [representable functor](../../../../../../representable-functor.md), it preserves small [categorical limits](../../../../../../categorical-limit.md). Part (b) makes $(1\downarrow G)$ have an [initial object](../../../../../../initial-object.md), which gives a [weakly initial set](../../../../../../weakly-initial-set.md).

Conversely, assume limit preservation and a [weakly initial set](../../../../../../weakly-initial-set.md) in $(1\downarrow G)$. The needed comma-limit fact is explicit: for a small [diagram in a category](../../../../../../diagram-category-theory.md) $(A_j,a_j)$, form $L=\lim_j A_j$ in $\mathcal C$. The elements $a_j\in G(A_j)$ form a compatible family, hence determine a unique $a\in G(L)$ under $G(L)\cong\lim_jG(A_j)$. The projections from $(L,a)$ are a [categorical limit](../../../../../../categorical-limit.md) in the [comma category](../../../../../../comma-category.md). This includes the empty diagram, since $G$ carries the [terminal object](../../../../../../terminal-object.md) to a singleton. Each comma [hom-set](../../../../../../hom-set.md) is a subset of a [hom-set](../../../../../../hom-set.md) in $\mathcal C$, so the [comma category](../../../../../../comma-category.md) is also [locally small](../../../../../../locally-small-category.md).

Part (c) now gives an [initial object](../../../../../../initial-object.md) of $(1\downarrow G)$, and part (b) supplies a [representation of a functor](../../../../../../representation-of-a-functor.md). Therefore

$$
\boxed{G\text{ is representable}\iff G\text{ preserves small limits and }(1\downarrow G)\text{ has a weakly initial set}.}
$$

The size requirement is a genuine [solution-set condition](../../../../../../solution-set-condition.md); limit preservation alone does not produce it in an arbitrary [complete category](../../../../../../complete-category.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
