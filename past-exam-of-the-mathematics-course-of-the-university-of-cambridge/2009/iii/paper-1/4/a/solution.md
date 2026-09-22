<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $m$ be the [order of a group element](../../../../../../order-of-a-group-element.md) $g$, allowing $m=\infty$. For finite $m$, take $C=\langle a\mid a^{nm}=1\rangle$; for infinite $m$, take $C=\langle a\mid\ \rangle\cong\mathbb Z$. Set

$$
G_1=G*C.
$$

The [normal form theorem for a free product](../../../../../../normal-form-theorem-for-a-free-product.md) embeds both factors, so $G$ is a [free factor](../../../../../../free-factor.md). The cyclic subgroup $A=\langle a^n\rangle$ has order $m$, just as $D=\langle g\rangle$ does. Hence $a^{nr}\mapsto g^r$ is a well-defined [group isomorphism](../../../../../../group-isomorphism.md) $A\to D$, and we may form the [HNN extension](../../../../../../hnn-extension.md)

$$
H=\langle G_1,t\mid t^{-1}a^nt=g\rangle.
$$

The single displayed conjugacy relation implements the full cyclic isomorphism by taking integer powers. [Britton's lemma](../../../../../../britton-s-lemma.md) embeds $G_1$ in $H$, so the original $G$ is preserved. Now take

$$
\boxed{h=t^{-1}at.}
$$

Cancellation of successive $tt^{-1}$ gives $h^n=t^{-1}a^nt=g$. This proves the [adjoining a root by an HNN extension](../../../../../../adjoining-a-root-by-an-hnn-extension.md) construction and all required embedding claims. If $g=1$, then $m=1$, $C=C_n$, and $A=D=\{1\}$; the HNN relation is vacuous and the same calculation gives $h^n=1$. The construction also works for $n=1$. It uses the actual order of $g$ as an existence parameter, not an algorithm for determining an unknown order.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
