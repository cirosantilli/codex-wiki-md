<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For all weights and biases collected in $\vartheta$, fit

$$
\min_\vartheta\left\{
-\sum_{i=1}^n\sum_{\ell=1}^LY_{i\ell}\log p_\ell(x_i;\vartheta)
+\lambda_1\lVert\vartheta\rVert_1+\lambda_2\lVert\vartheta\rVert_2^2
\right\}.
$$

Use backpropagation with stochastic gradient descent or a modern adaptive variant, treating the absolute-value derivative at zero as stated. Select $(\lambda_1,\lambda_2)$ by validation or cross-validation and refit using the selected pair.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
