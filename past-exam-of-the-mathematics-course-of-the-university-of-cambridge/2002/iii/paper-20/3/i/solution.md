<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [functor](../../../../../../functor.md) $D:\mathcal J\to\mathcal C$ with finite indexing [category](../../../../../../category-split.md), form the finite [products in a category](../../../../../../product-category-theory.md)

$$
P=\prod_{j\in\operatorname{Ob}\mathcal J}D(j),\qquad Q=\prod_{u:i\to j\text{ in }\mathcal J}D(j).
$$

Define $s,t:P\rightrightarrows Q$ by requiring the coordinate indexed by $u:i\to j$ to be $D(u)\pi_i$ for $s$ and $\pi_j$ for $t$. Let $e:L\to P$ be their [equalizer](../../../../../../equaliser.md), and put $\lambda_j=\pi_j e$. The equality $se=te$ says exactly that $D(u)\lambda_i=\lambda_j$ for every [morphism](../../../../../../morphism.md) $u$, so these [morphisms](../../../../../../morphism.md) form a [categorical cone](../../../../../../cone-over-a-diagram.md).

For any other [categorical cone](../../../../../../cone-over-a-diagram.md) $(x_j:X\to D(j))$, the [product in a category](../../../../../../product-category-theory.md) gives a unique $x:X\to P$ with $\pi_jx=x_j$. The [categorical cone](../../../../../../cone-over-a-diagram.md) equations give $sx=tx$, so the [equalizer](../../../../../../equaliser.md) gives a unique $\bar x:X\to L$ with $e\bar x=x$. This is exactly the [universal property](../../../../../../universal-property.md) of a [categorical limit](../../../../../../categorical-limit.md). Empty indexing products are [terminal objects](../../../../../../terminal-object.md), so the construction includes the empty [diagram in a category](../../../../../../diagram-category-theory.md). Thus **finite products and [equalizers](../../../../../../equaliser.md) give all [finite limits](../../../../../../finite-limit.md)**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
