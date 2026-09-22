<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose $(\lambda_1,\lambda_2)$ on a grid by [K-fold cross-validation](../../../../../../k-fold-cross-validation.md), comparing the same held-out prediction loss and optionally applying the one-standard-error rule for a simpler model. A genuinely untouched [test set](../../../../../../test-set.md) can then estimate final prediction error.

Ordinary model-based intervals after selecting nonzero coefficients ignore selection and are generally invalid. Valid approaches include [Debiased Lasso](../../../../../../debiased-lasso.md) or a selective-inference procedure under its assumptions, sample splitting followed by an unpenalized refit and inference on the independent half, or a bootstrap that repeats both tuning and fitting and is interpreted with care near the nonsmooth zero threshold.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
