<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Writing $\eta_i=\beta_0+x_i^T\beta$, the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta_0,\beta)
=\sum_{i=1}^n
\left\{y_i\eta_i-\log(1+e^{\eta_i})\right\}.
$$

With 500 observations and 5000 word predictors, the augmented design matrix cannot have full column rank. There are nonzero coefficient directions that leave every $\eta_i$ unchanged, so any maximizer belongs to an affine family and is not unique. In addition, the high-dimensional features may completely separate the classes, in which case no finite maximizer exists at all.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
