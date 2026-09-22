<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

A [pi-system](../../../../../pi-system.md) is a collection closed under finite intersections. The uniqueness theorem says that two [probability](../../../../../probability.md) measures agreeing on a generating [pi-system](../../../../../pi-system.md) agree on its generated sigma-field. For finite measures one also fixes the total [mass](../../../../../mass.md); for a sigma-finite version one requires a covering sequence from the [pi-system](../../../../../pi-system.md) with finite common [masses](../../../../../mass.md). Adding the whole space to a [pi-system](../../../../../pi-system.md) of events causes no change to its generated sigma-field and preserves the stated independence condition.

Fix $H\in\mathcal H$. On $\sigma(\mathcal G)$ the finite measures $A\mapsto P(A\cap H)$ and $A\mapsto P(A)P(H)$ agree on $\mathcal G$ and on the whole space. Uniqueness makes them agree for every $A\in\sigma(\mathcal G)$. Now fix such an $A$. On $\sigma(\mathcal H)$ the measures $B\mapsto P(A\cap B)$ and $B\mapsto P(A)P(B)$ agree on $\mathcal H$ and the whole space; a second application of uniqueness proves

$$
\boxed{P(A\cap B)=P(A)P(B)\quad(A\in\sigma(\mathcal G),\ B\in\sigma(\mathcal H)).}
$$

Thus the two generated sigma-fields are independent. The extension is done one argument at a time, not by assuming the required independence for arbitrary unions.

For the [independent random variables](../../../../../independent-random-variables.md), let $\mathcal G$ be the rectangles $\bigcap_{i=1}^m\{Y_i\in B_i\}$ and let $\mathcal H$ be the analogous rectangles in the $Z_j$. Both are [pi-systems](../../../../../pi-system.md). Joint independence of the full list factors each combined rectangular [probability](../../../../../probability.md) into the product of the individual [probabilities](../../../../../probability.md), hence into $P(G)P(H)$. Their generated sigma-fields are exactly $\sigma(Y_1,\ldots,Y_m)$ and $\sigma(Z_1,\ldots,Z_n)$. The proved result therefore gives **independence of the two vector-generated sigma-fields**.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
