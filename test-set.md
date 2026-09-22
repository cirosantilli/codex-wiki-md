# Test set

↑ **Parent:** [Validation set](validation-set.md)

A test set is held out from both parameter fitting and [model selection](model-selection.md) and is used to estimate the final selected procedure's [prediction error](prediction-error.md). A [validation set](validation-set.md) influences the choice; a [test set](test-set.md) assesses that choice after it is fixed. The distinction concerns how observations are used, not their file names.

For a fixed rule and an [independent](independent-random-variables.md) [test set](test-set.md) of size $m$ from the target [probability distribution](probability-distribution.md),

$$
\widehat R_{\mathrm{test}}=\frac1m\sum_{j=1}^m L(Y_j^*,\widehat f(X_j^*)),\qquad
\mathbb E[\widehat R_{\mathrm{test}}\mid\mathcal D_n]=R(\widehat f).
$$

This [test error](test-error.md) is an estimate, with sampling uncertainty; it is not a guarantee for each future prediction. [Dataset shift](dataset-shift.md) changes what performance the estimate represents.

In the [overfitting](overfitting.md) example, all degree choices are fixed in advance, [cross-validation](cross-validation.md) uses only [training data](training-data.md), and the selected degree is locked before evaluating 400 separate points. Displaying the other curves afterward explains their behavior; it does not authorize selecting by those scores. Repeatedly inspecting a [test set](test-set.md) and changing the model makes it part of [model selection](model-selection.md), introducing [data leakage](data-leakage.md) and potentially optimistic assessment. [Cawley and Talbot, over-fitting in model selection, 2010](https://jmlr.org/papers/v11/cawley10a.html)

## ↑ Ancestors (8)

1. [Validation set](validation-set.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Cost-complexity tree pruning](cost-complexity-tree-pruning.md)
- [Cross-validation](cross-validation.md)
- [Misclassification rate](misclassification-rate.md)
- [Overfitting](overfitting.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218/5/e/solution.md)
- [Ridge regression](ridge-regression.md)
- [Statistical learning](statistical-learning-split.md)
- [Test set](test-set.md)
- [Underfitting](underfitting.md)
