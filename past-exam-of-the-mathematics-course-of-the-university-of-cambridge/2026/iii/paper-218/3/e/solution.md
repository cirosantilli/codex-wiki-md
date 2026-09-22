<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The code computes [Leave-one-out cross-validation](../../../../../../leave-one-out-cross-validation.md). If

$$
Y_i(\widehat\alpha+X_i^\top\widehat\beta)>1,
$$

then observation $i$ is not a support vector. Removing it leaves the optimum unchanged, and the resulting classifier still classifies it correctly. A leave-one-out error can therefore occur only for an observation on or inside the margin, which proves

$$
\widehat{\operatorname{Err}}
\leq\frac1n\sum_{i=1}^n
\mathbf1_{\{Y_i(\widehat\alpha+X_i^\top\widehat\beta)\leq1\}}.
$$

Thus the fraction of training observations on or inside the margin is an upper bound on leave-one-out error. One can refit only after deleting support vectors, reusing the full fit for every other observation. Alternatively, [K-fold cross-validation](../../../../../../k-fold-cross-validation.md) needs only $K$ fits and is often preferable for larger data sets.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
