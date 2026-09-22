<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The classification form of [CART](../../../../../../classification-and-regression-tree.md) starts with the root rectangle $R=[0,1]^2$. For any current region $A$, let $N(A)=\#\{i:X_i\in A\}$ and let

$$
\widehat p(A)=\frac{\#\{i:X_i\in A,\,Y_i=\text{circle}\}}{N(A)},
\qquad
G(A)=\widehat p(A)(1-\widehat p(A))
$$

be its empirical class proportion and [Gini impurity](../../../../../../gini-impurity.md). A candidate axis-aligned split $X_j\leq s$ partitions $R$ into $U$ and $V$. Its impurity change is

$$
Q=\frac{N(U)}{N(R)}G(U)
+\frac{N(V)}{N(R)}G(V)-G(R).
$$

Among all coordinates and thresholds between consecutive observed coordinates, CART chooses a split minimizing $Q$, then applies the same [recursive partitioning](../../../../../../recursive-partitioning.md) independently to the children until a stopping rule is met. Each terminal region predicts its majority class. Pruning may then select a smaller subtree by penalizing the number of leaves.

For the resulting classifier $\widehat C$, the [training error](../../../../../../training-error.md) is

$$
\widehat R_{train}=\frac19\sum_{i=1}^9
\mathbf1_{\{\widehat C(X_i)\ne Y_i\}},
$$

while its [prediction error](../../../../../../prediction-error.md) is $R(\widehat C)=\mathbb P\{\widehat C(X_{new})\ne Y_{new}\}$ for an independent observation drawn from the target population.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
