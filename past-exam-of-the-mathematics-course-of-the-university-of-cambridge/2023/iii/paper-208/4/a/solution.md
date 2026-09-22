<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix every coordinate except $X_i$. As $X_i$ varies, the [longest increasing subsequence](../../../../../../longest-increasing-subsequence.md) length can change by at most one: deleting the changed term leaves a common subsequence of length at least the larger value minus one. The conditional range therefore has length at most one, so the [Popoviciu inequality on variances](../../../../../../popoviciu-s-inequality-on-variances.md) gives

$$
\operatorname{Var}(Z\mid X^{(i)})\leq\frac14.
$$

The coordinatewise conditional-variance form of the [Efron–Stein inequality](../../../../../../efron-stein-inequality.md) now yields

$$
\boxed{\operatorname{Var}(Z)
\leq\sum_{i=1}^n\mathbb E[\operatorname{Var}(Z\mid X^{(i)})]
\leq\frac n4.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
