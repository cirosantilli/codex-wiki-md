<h1 id="30j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [regression tree](../../../../../../regression-tree.md) chooses a threshold $s$ and constant predictions $c_L,c_R$ to minimize the squared-error criterion

$$
\min_{s,c_L,c_R}
\left\{
\sum_{i:X_i\leq s}(Y_i-c_L)^2
+\sum_{i:X_i>s}(Y_i-c_R)^2
\right\},
$$

where $s$ ranges over thresholds producing two nonempty groups. For a fixed split, the [least-squares](../../../../../../ordinary-least-squares-estimators.md) minimizers are the two sample means,

$$
c_L=\frac{1}{n_L}\sum_{X_i\leq s}Y_i,
\qquad
c_R=\frac{1}{n_R}\sum_{X_i>s}Y_i.
$$

**Thus the first split is the candidate threshold with the smallest sum of the two within-node residual sums of squares.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
