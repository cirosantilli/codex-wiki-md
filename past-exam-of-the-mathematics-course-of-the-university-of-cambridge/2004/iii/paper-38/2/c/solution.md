<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $D=\sum_{j=1}^n\mathbf1_{\{T_j\le c_j\}}$ be the observed event count. For each subject, the fixed-censoring identity gives $\mathbb EH(X_j)=\mathbb P(T_j\le c_j)$. [Linearity of expectation](../../../../../../linearity-of-expectation.md) therefore yields

$$
\boxed{\mathbb E\sum_{j=1}^nH(X_j)=\sum_{j=1}^n\mathbb P(T_j\le c_j)=\mathbb ED.}
$$

[Independence](../../../../../../independent-random-variables.md) between subjects is not needed for this [expectation](../../../../../../expected-value.md) identity. The common $H$ presumes a common marginal [hazard](../../../../../../hazard-function.md); with heterogeneous subject-specific [hazards](../../../../../../hazard-function.md), replace it by $H_j$ for subject $j$. Random [censoring](../../../../../../censoring-statistics.md) admits the analogous conditional argument when its [independence](../../../../../../independent-random-variables.md) assumptions hold.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
