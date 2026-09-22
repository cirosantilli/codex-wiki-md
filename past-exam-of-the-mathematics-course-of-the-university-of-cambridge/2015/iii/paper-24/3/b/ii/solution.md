<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [diamond theorem in the constructible universe](../../../../../../../diamond-theorem-in-the-constructible-universe.md) gives $L\models\diamondsuit$, and $L$ satisfies [ZFC](../../../../../../../zermelo-fraenkel-set-theory-with-choice.md). Apply the preceding construction inside $L$ with $S=\omega_1^L$. It produces a normal splitting [Suslin tree](../../../../../../../suslin-tree.md).

For completeness, such a tree yields a [Suslin line](../../../../../../../suslin-line.md). Order its nodes lexicographically using the two successors at every split, treating a node itself as a position between its two successor subtrees. Each node is thus a cut point between a left and a right subtree. This gives a [dense linear order without endpoints](../../../../../../../dense-linear-order-without-endpoints.md). Every nonempty interval contains a whole cone above some node: for comparable endpoints use the successor cone of the descendant endpoint directed toward the other endpoint; for incomparable endpoints use the right-successor cone of the lower endpoint. Disjoint intervals therefore supply pairwise incomparable cone roots, so the order has the [countable chain condition for a linear order](../../../../../../../countable-chain-condition-for-a-linear-order.md). A countable collection of nodes has bounded heights; a cone based above that bound contains none of them, so it is not an [order-dense subset](../../../../../../../order-dense-subset.md). Passing to the [Dedekind completion](../../../../../../../dedekind-completion.md) using proper cuts, so that no endpoints are added, preserves density, the [countable chain condition for a linear order](../../../../../../../countable-chain-condition-for-a-linear-order.md), and nonseparability. For nonseparability, a countable dense set in the completion would give a countable dense set of original nodes by choosing one original node between each distinct pair of its points. This contradicts the preceding height-bound argument. The result is a [Suslin line](../../../../../../../suslin-line.md).

Thus the [Suslin hypothesis](../../../../../../../suslin-hypothesis.md) fails in $L$. The [constructible universe theorem](../../../../../../../constructible-universe-theorem.md) is a theorem of [ZFC](../../../../../../../zermelo-fraenkel-set-theory-with-choice.md), so this is a relative-consistency argument, without an additional assumption that a transitive model exists:

$$
\boxed{\operatorname{Con}(\mathrm{ZFC})\Longrightarrow
\operatorname{Con}(\mathrm{ZFC}+\neg\mathrm{SH}).}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
