<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The intended quantity is the [Leave-one-out cross-validation](../../../../../../leave-one-out-cross-validation.md) error

$$
\operatorname{LOOCV}
=\frac1n\sum_{i=1}^n
\ell\!\left(\widehat h^{(-i)}(X_i),Y_i\right),
$$

where $\widehat h^{(-i)}$ is trained without observation $i$ and the loss is the zero-one misclassification loss. Computing it literally requires fitting $10000$ neural networks, which is prohibitively expensive.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
