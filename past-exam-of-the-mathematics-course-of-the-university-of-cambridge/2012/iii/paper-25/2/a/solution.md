<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D:J\to\mathcal C$ be a finite [diagram in a category](../../../../../../diagram-category-theory.md). Form the finite [products in a category](../../../../../../product-category-theory.md)

$$
P=\prod_{j\in\operatorname{Ob}J}D(j),\qquad Q=\prod_{a:j\to k\ \text{in }J}D(k).
$$

Define $s,t:P\rightrightarrows Q$ by $\pi_a s=D(a)\pi_j$ and $\pi_a t=\pi_k$. Take their [equalizer](../../../../../../equaliser.md) $e:L\to P$. The maps $\lambda_j=\pi_j e$ satisfy $D(a)\lambda_j=\lambda_k$, so they constitute a [categorical cone](../../../../../../cone-over-a-diagram.md).

Any other [categorical cone](../../../../../../cone-over-a-diagram.md) $x_j:X\to D(j)$ gives a unique $x:X\to P$ by the [product in a category](../../../../../../product-category-theory.md) property. Its cone equations say $sx=tx$, so the [equalizer](../../../../../../equaliser.md) gives a unique $\bar x:X\to L$ with $e\bar x=x$. The projections then give $\lambda_j\bar x=x_j$, and uniqueness follows from both universal properties. Thus **this [equalizer](../../../../../../equaliser.md) of two product maps is the [finite limit](../../../../../../finite-limit.md) of the [diagram in a category](../../../../../../diagram-category-theory.md)**.

The empty indexing [category](../../../../../../category-split.md) is included: its empty [product in a category](../../../../../../product-category-theory.md) is a [terminal object](../../../../../../terminal-object.md), which is the empty [categorical limit](../../../../../../categorical-limit.md). Hence no nonemptiness restriction has entered the construction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
