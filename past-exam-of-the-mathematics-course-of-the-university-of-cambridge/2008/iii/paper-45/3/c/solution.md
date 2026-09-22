<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [random forest](../../../../../../random-forest.md) constructs an ensemble of [classification and regression trees](../../../../../../classification-and-regression-tree.md). For each tree, draw a [bootstrap](../../../../../../bootstrapping-statistics.md) sample of the training observations. Grow the tree by [recursive partitioning](../../../../../../recursive-partitioning.md); at each node, draw a fresh random subset of predictor coordinates and choose the best split only among those coordinates, using a criterion such as [Gini impurity](../../../../../../gini-impurity.md). Trees are ordinarily grown deeply with a chosen minimum terminal-node size and without the pruning used to select a single small tree. Repeat for many independently randomized trees. For binary classification, predict by [majority vote](../../../../../../majority-vote.md); for regression, average the tree predictions. The [out-of-bag error](../../../../../../out-of-bag-error.md) predicts each observation using only trees whose bootstrap samples omitted it, furnishing an internal assessment of prediction error.

The strategies differ in how they form a useful ensemble. The forest uses resampling and random predictor subsets to decorrelate trees; averaging then reduces the variability of individual tree predictions. For illustration, if equally weighted predictions have common variance $v$ and pairwise correlation $\rho$, the variance of their average is $v[\rho+(1-\rho)/M]$, showing why low inter-tree correlation matters. This identity describes a regression-prediction calculation; it is not an exact classification-error formula.

[AdaBoost](../../../../../../adaboost.md) instead fits sequentially, with each round responding to errors of the accumulated score. It uses nonuniform observation weights and nonuniform final classifier weights derived from exponential loss; a forest's bootstrap sampling is ordinarily uniform and its final votes are ordinarily equal. Forest trees can be built in parallel once the data and tuning parameters are fixed, whereas each boosting stage depends on previous stages. Random forests commonly use deep trees; AdaBoost often uses shallow trees or stumps as [weak learners](../../../../../../weak-learner.md), although its base class is not restricted to them. Reweighting persistent errors can make boosting sensitive to mislabeled points and outliers, while randomization and averaging often make a forest less sensitive; neither statement is a universal robustness theorem. Both methods require attention to ensemble size and tree complexity, and neither guarantees a better classifier for every dataset.

**Random forests diversify and average randomized trees; AdaBoost sequentially fits errors and combines classifiers with loss-derived weights.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
