<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $D:J\to[\mathcal C,\mathcal S]$ be a small [diagram in a category](../../../../../../diagram-category-theory.md). Since $\mathcal S$ is a [complete category](../../../../../../complete-category.md), choose at each $C\in\mathcal C$ a [categorical limit](../../../../../../categorical-limit.md)

$$
L(C)=\lim_{j\in J}D_j(C),\qquad p_{j,C}:L(C)\to D_j(C).
$$

For $f:C\to C'$, the arrows $D_j(f)p_{j,C}$ form a [cone over a diagram](../../../../../../cone-over-a-diagram.md) at $C'$, because the diagram arrows $D_j\to D_k$ are [natural transformations](../../../../../../natural-transformation.md). There is therefore a unique arrow $L(f):L(C)\to L(C')$ with

$$
p_{j,C'}L(f)=D_j(f)p_{j,C}.
$$

The [universal property](../../../../../../universal-property.md) immediately gives $L(1_C)=1_{L(C)}$ and $L(gf)=L(g)L(f)$: both sides have the same composites with every limit projection. Thus $L$ is a [functor](../../../../../../functor.md), and the displayed equations make the $p_j$ [natural transformations](../../../../../../natural-transformation.md).

Given any [categorical cone](../../../../../../cone-over-a-diagram.md) $q_j:X\to D_j$ in the [functor category](../../../../../../functor-category.md), its components induce unique $q_C:X(C)\to L(C)$. For $f:C\to C'$, compare $L(f)q_C$ and $q_{C'}X(f)$ after each $p_{j,C'}$; [naturality](../../../../../../naturality.md) of $q_j$ makes their composites equal. Hence $q$ is a [natural transformation](../../../../../../natural-transformation.md), and uniqueness is componentwise. This proves that $L$ is a [categorical limit](../../../../../../categorical-limit.md) in $[\mathcal C,\mathcal S]$.

**The functor category is complete, and every evaluation functor preserves limits**, since evaluating the constructed limit at $C$ gives exactly the chosen limit in $\mathcal S$. This is the [pointwise limits in a functor category](../../../../../../pointwise-limits-in-a-functor-category.md) construction; it also covers the empty diagram and its [terminal object](../../../../../../terminal-object.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
