<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose $G=\langle g_1,\ldots,g_n\mid R\rangle$ has a [finite group presentation](../../../../../../finite-group-presentation.md). Work in the [free product](../../../../../../free-product.md) $B=G*F(a,b)$ and put

$$
u_0=a,\quad u_i=b^{-i}ab^i,\qquad
v_0=b,\quad v_i=g_i a^{-i}ba^i\quad(1\le i\le n).
$$

The $u_i$ freely generate a subgroup of $F(a,b)$. Indeed, in a reduced word in these conjugates, combine adjacent powers with the same index. Expanding the remaining word leaves nonzero powers of $a$ separated by nonzero powers of $b$, so the [normal form theorem for a free product](../../../../../../normal-form-theorem-for-a-free-product.md) makes it nonidentity. This proves the [free conjugate bases in a rank-two free group](../../../../../../free-conjugate-bases-in-a-rank-two-free-group.md) fact we need.

The [group homomorphism](../../../../../../group-homomorphism.md) $B\to F(a,b)$ killing $G$ sends $v_i$ to $a^{-i}ba^i$, including $v_0=b$. These are a free conjugate basis by the same argument with $a,b$ interchanged. A nonempty reduced word in the $v_i$ therefore has nontrivial image and cannot be trivial in $B$. Thus $u_i\mapsto v_i$ extends to an [isomorphism](../../../../../../isomorphism.md) between the two rank-$(n+1)$ [free groups](../../../../../../free-group.md) embedded in $B$.

Adjoin one [stable letter](../../../../../../stable-letter.md) implementing this isomorphism:

$$
E=\langle g_1,\ldots,g_n,a,b,t\mid R,\ t^{-1}u_it=v_i\ (0\le i\le n)\rangle.
$$

We assume [Britton's lemma](../../../../../../britton-s-lemma.md), including its assertion that the base embeds in this [HNN extension](../../../../../../hnn-extension.md), and the factor-embedding assertion of the [normal form theorem for a free product](../../../../../../normal-form-theorem-for-a-free-product.md). Hence $G\hookrightarrow E$. The presentation is finite, and its relations express every generator in $a,t$:

$$
b=t^{-1}at,\qquad
g_i=t^{-1}b^{-i}ab^it\,(a^{-i}ba^i)^{-1}.
$$

Eliminating $b,g_i$ by [Tietze transformations](../../../../../../tietze-transformations.md) therefore gives **a two-generator finite presentation with $\boxed{G\hookrightarrow E=\langle a,t\rangle}$**. This explicitly constructs the [two-generator HNN embedding](../../../../../../two-generator-hnn-embedding.md); it does not rely on an arbitrary two-generator embedding preserving finite presentability.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
