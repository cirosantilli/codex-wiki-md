<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose $\lambda$ to minimize an estimate of out-of-sample [mean squared prediction error](../../../../../../mean-squared-prediction-error.md), commonly [K-fold cross-validation](../../../../../../k-fold-cross-validation.md) or a separate [validation set](../../../../../../validation-set.md). As $\lambda$ increases, the coefficient vector is shrunk toward zero. This generally increases [bias of an estimator](../../../../../../bias-of-an-estimator.md) but decreases [variance of an estimator](../../../../../../variance-of-an-estimator.md); the minimizing value balances the two contributions in the [bias-variance tradeoff](../../../../../../bias-variance-tradeoff.md). The independent test set in the question can assess the final choice, but repeatedly selecting $\lambda$ on that same set would cause [data leakage](../../../../../../data-leakage.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
