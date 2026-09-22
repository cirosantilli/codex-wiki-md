<h1 id="15/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Initialize the weights, evaluate the feature matrix and repeat [gradient descent](../../../../../gradient-descent-split.md) updates until the loss or gradient stabilizes. If $\widetilde{\mathbf z}_i=(1,\mathbf z_i)$ includes the intercept, then

$$
\nabla\mathcal L=\frac1m\sum_i(h_i-y_i)\widetilde{\mathbf z}_i,
\qquad
\mathbf w\leftarrow\mathbf w-\eta\nabla\mathcal L.
$$

A positive step size $\eta$ chosen by a convergence rule or [line search](../../../../../line-search.md) gives a practical optimization algorithm. Mini-batch updates or a Newton-type method are alternatives. Fit feature scaling, choose regularization and choose any nonstandard threshold using training or validation data, then freeze the procedure before using the held-out test set.

For $M$ held-out examples, set $\widehat Y_i=\mathbf1\{h(\mathbf Z_i;\widehat{\mathbf w})\geq t\}$, with $t=0.5$ unless selected otherwise. The requested [classification accuracy](../../../../../classification-accuracy.md) is

$$
\boxed{\mathrm{accuracy}=\frac1M\sum_{i=1}^M\mathbf1\{\widehat Y_i=Y_i\}
=\frac{TP+TN}{TP+TN+FP+FN}.}
$$

**Always predicting the majority class already gives about 90% accuracy.** Report a [confusion matrix](../../../../../confusion-matrix.md), [classification recall](../../../../../recall-classification.md) and [classification precision](../../../../../precision-classification.md) as well, especially for the minority class. A [precision-recall curve](../../../../../precision-recall-curve.md) shows the threshold tradeoff without confusing high majority-class accuracy with successful minority-class detection. No numerical test accuracy can be calculated without the held-out predictions and labels.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
