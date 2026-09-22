<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D:I\to\mathcal C$ be a finite diagram. Form the finite [categorical products](../../../../../../product-category-theory.md)

$$
P=\prod_{i\in\operatorname{Ob}I}D(i),\qquad Q=\prod_{u:i\to j\in\operatorname{Mor}I}D(j).
$$

There are two [morphisms](../../../../../../morphism.md) $s,t:P\rightrightarrows Q$: their components at $u:i\to j$ are $D(u)\pi_i$ and $\pi_j$, respectively. Let $e:L\to P$ be their [equaliser](../../../../../../equaliser.md). Then $\ell_i=\pi_i e$ satisfy $D(u)\ell_i=\ell_j$, so they constitute a [cone over a diagram](../../../../../../cone-over-a-diagram.md).

Any other cone $x_i:X\to D(i)$ uniquely determines $x:X\to P$. Its cone equations say precisely that $sx=tx$. The [equaliser](../../../../../../equaliser.md) therefore gives a unique $h:X\to L$ with $eh=x$, and thus $\ell_i h=x_i$. Conversely these component equations force $eh=x$ by the [categorical product](../../../../../../product-category-theory.md) [universal property](../../../../../../universal-property.md), so there is exactly one such mediator. This proves that $(L,\ell_i)$ is a [categorical limit](../../../../../../categorical-limit.md) of $D$.

The empty [categorical products](../../../../../../product-category-theory.md) are included: if $I$ is empty, $P$ and $Q$ are terminal and the construction gives the empty [categorical limit](../../../../../../categorical-limit.md). Thus **finite [categorical products](../../../../../../product-category-theory.md) and [equalisers](../../../../../../equaliser.md) give every finite [categorical limit](../../../../../../categorical-limit.md)**, as a special case of the [construction of small limits from products and equalizers](../../../../../../construction-of-small-limits-from-products-and-equalizers.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
