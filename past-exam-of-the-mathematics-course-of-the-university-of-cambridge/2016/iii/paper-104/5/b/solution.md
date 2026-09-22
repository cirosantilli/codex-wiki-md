<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a [reduced sequence in an HNN extension](../../../../../../reduced-sequence-in-an-hnn-extension.md) for $\gamma$. By repeatedly conjugating a prefix to the other end and reducing any resulting pinch, one obtains a [cyclically reduced sequence in an HNN extension](../../../../../../cyclically-reduced-sequence-in-an-hnn-extension.md): either an element of the base group, or a sequence of positive stable-letter length with no pinch even across its cyclic junction. For example, after conjugating away the initial base coefficient, write it as $t^{\epsilon_1}g_1\cdots t^{\epsilon_k}g_k$. A pinch across the junction can occur only if $\epsilon_k=-\epsilon_1$ and $g_k\in C_{\epsilon_k}$. Moving the first stable letter to the end then exposes that pinch and reduces the stable-letter length by two. Iteration must terminate.

If the resulting cyclically reduced sequence has $k>0$, every positive power remains reduced and has stable-letter length equal to that power times $k$. By [Britton's lemma](../../../../../../britton-s-lemma.md), none is the identity. Thus a finite-order element must be conjugate into the base group $G$. Since $G$ embeds in the [HNN extension](../../../../../../hnn-extension.md), the order of a base-group element is unchanged, and conjugation also preserves order. Therefore

$$
\boxed{\gamma\text{ has finite order}\iff\gamma\text{ is conjugate to a finite-order element of }G.}
$$

The argument also applies to several stable letters: cyclic pinches must involve a stable letter and its own inverse.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 104](../../../paper-104-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
