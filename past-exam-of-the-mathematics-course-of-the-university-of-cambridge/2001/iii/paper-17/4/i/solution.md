<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First construct every finite [product in a category](../../../../../../product-category-theory.md) by iterating binary [products in a category](../../../../../../product-category-theory.md); the empty product is the [terminal object](../../../../../../terminal-object.md). Let $D:J\to\mathcal C$ be a [diagram in a category](../../../../../../diagram-category-theory.md) with finitely many objects and arrows. Form the finite [products in a category](../../../../../../product-category-theory.md)

$$
P=\prod_{j\in\operatorname{Ob}J}D(j),\qquad
Q=\prod_{u:i\to j\text{ in }J}D(j).
$$

Define $a,b:P\rightrightarrows Q$ by their components

$$
\pi_u a=D(u)\pi_i,\qquad \pi_u b=\pi_j.
$$

Take their [equalizer](../../../../../../equaliser.md) $e:L\to P$. Its components $p_j=\pi_j e$ satisfy $D(u)p_i=p_j$, so they form a [cone over a diagram](../../../../../../cone-over-a-diagram.md).

For any other [categorical cone](../../../../../../cone-over-a-diagram.md) $x_j:X\to D(j)$, the [product in a category](../../../../../../product-category-theory.md) property supplies a unique $x:X\to P$ with $\pi_jx=x_j$. The cone equations imply $ax=bx$, so the [equalizer](../../../../../../equaliser.md) property supplies a unique $\bar x:X\to L$ with $e\bar x=x$. These are exactly the required equations $p_j\bar x=x_j$, with uniqueness. Thus $L$ is a [categorical limit](../../../../../../categorical-limit.md). For empty $J$, both products are terminal and this construction still gives a terminal limit. **All finite limits exist.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
