<h1 id="6/a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Suppose $w\ne1$ in $P$. In $D=P*F(z,d)$, the [commutator](../../../../../../../commutator.md) $c=wzw^{-1}z^{-1}$ is a nonempty cyclically alternating free-product word. Every positive power remains reduced, so $c$ has infinite order. Each $g_j$ also has infinite order: this is immediate for $z,d$; if $x_i=1$, then $x_i z=z$, and otherwise $x_i z$ is a cyclically alternating word of length two.

Consequently the presentation defining $H$ is a multiple [HNN extension](../../../../../../../hnn-extension.md) identifying the infinite cyclic subgroups $\langle c\rangle$ and $\langle g_j\rangle$. By the [normal form theorem for an HNN extension](../../../../../../../normal-form-theorem-for-an-hnn-extension.md), $D$ embeds in $H$.

The subgroup

$$
U=\langle C,u_0,\ldots,u_{n+1}\rangle\le H
$$

is a [free group](../../../../../../../free-group.md) on exactly these $n+3$ elements. For a proof, view $D$ as $(P*\langle z\rangle)*\langle d\rangle$. For every $k\ne0$, the reduced expression $C^k=d^{-1}c^kd$ lies neither in $P*\langle z\rangle$ nor in $\langle d\rangle$. It therefore belongs to none of the associated cyclic subgroups $\langle c\rangle$ or $\langle g_j\rangle$. Any freely reduced word in $C,u_0,\ldots,u_{n+1}$ with a stable letter has no pinch and is nontrivial by [Britton's lemma](../../../../../../../britton-s-lemma.md). A word with no stable letters is a nonzero power of $C$, also nontrivial. This proves the claimed [free basis of a group](../../../../../../../free-basis-of-a-group.md).

Inside the rank-two [free group](../../../../../../../free-group.md) $\langle a_1,a_3\rangle\le Q$, the elements

$$
a_1,\ a_3a_1a_3^{-1},\ldots,\ a_3^{n+2}a_1a_3^{-(n+2)}
$$

freely generate a subgroup $V$ of rank $n+3$. This is the same free-product normal-form calculation as for the conjugate basis in Question 5: between conjugates with distinct indices, a nonzero power of $a_3$ remains. The identifications in the output presentation give an [isomorphism](../../../../../../../isomorphism.md) $U\to V$ matching these free bases. Hence

$$
P(w)\cong H*_{U=V}Q.
$$

The [normal form theorem for an amalgamated free product](../../../../../../../normal-form-theorem-for-an-amalgamated-free-product.md) makes both factors embed. Composing the embeddings gives

$$
\boxed{P\hookrightarrow D\hookrightarrow H\hookrightarrow P(w).}
$$

Thus the construction preserves $P$ whenever the input word is nontrivial, regardless of whether that word has finite or infinite order in $P$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 104](../../../../paper-104-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
