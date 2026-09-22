<h1 id="13e/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The labels (i) and (ii) in the original PDF are hypotheses of one theorem, not separate requests. Here is the finite-cover step furnished by the [compact](../../../../../../../compact-space.md) fibres. Start with any [open cover](../../../../../../../open-cover.md) $\{U_i\}_{i\in I}$ of $f^{-1}(K)$, with the $U_i$ open in $X$ (a relative cover can be lifted to one of this form). For each $y\in K$, [compactness](../../../../../../../compact-space.md) gives a finite set $I_y\subseteq I$ with

$$
f^{-1}(\{y\})\subseteq V_y:=\bigcup_{i\in I_y}U_i.
$$

An empty fibre needs no cover elements: take $I_y=\varnothing$ and $V_y=\varnothing$.

The complementary set $A_y=X\setminus V_y$ is [closed set](../../../../../../../closed-set.md). By the [closed map](../../../../../../../closed-map.md) hypothesis, its image is [closed set](../../../../../../../closed-set.md), so

$$
W_y:=Y\setminus f(A_y)
$$

is open, contains $y$, and satisfies $f^{-1}(W_y)\subseteq V_y$. These open sets cover the [compact set](../../../../../../../compact-space.md) $K$. Select finitely many, $W_{y_1},\ldots,W_{y_m}$. The finitely many original cover elements with indices in $I_{y_1}\cup\cdots\cup I_{y_m}$ then cover $f^{-1}(K)$. Therefore

$$
\boxed{f^{-1}(K)\text{ is compact}}.
$$

This proves the unheaded conclusion in the PDF as well as explaining the role of hypothesis (i). No [Hausdorff](../../../../../../../hausdorff-space.md) assumption is needed for this [compact-preimage theorem for closed maps](../../../../../../../compact-preimage-theorem-for-closed-maps.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [13E](../../../13e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
