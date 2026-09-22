# One-nearest-neighbour asymptotic risk

↑ **Parent:** [One-nearest-neighbour classifier](one-nearest-neighbour-classifier.md)

For [binary classification](binary-classification.md), write $\eta(x)=\mathbb P(Y=1\mid X=x)$ and assume [feature-measurable nearest-neighbour tie-breaking](feature-measurable-nearest-neighbour-tie-breaking.md). If $\mathbb E|\eta(X_{(1)}(X))-\eta(X)|\to0$, then the expected [conditional misclassification risk](conditional-misclassification-risk.md) of the [one-nearest-neighbour classifier](one-nearest-neighbour-classifier.md) tends to $\mathbb E[2\eta(X)(1-\eta(X))]$. Couple each label and an oracle label using one uniform variable. Their disagreement has the preceding expected absolute difference. The oracle and the test label are conditionally [independent](independent-random-variables.md) [Bernoulli random variables](bernoulli-distribution.md) of parameter $\eta(X)$, so their disagreement [probability](probability.md) is exactly $2\eta(X)(1-\eta(X))$. The difference of [classification in statistical learning](classification-in-statistical-learning.md) error probabilities is at most the coupling disagreement.

**Table of contents**

- [Bayes risk bound for one-nearest-neighbour classification](bayes-risk-bound-for-one-nearest-neighbour-classification.md)

## ↑ Ancestors (10)

1. [One-nearest-neighbour classifier](one-nearest-neighbour-classifier.md)
2. [K-nearest neighbors algorithm](k-nearest-neighbors-algorithm.md)
3. [Classification in statistical learning](classification-in-statistical-learning.md)
4. [Statistical learning](statistical-learning-split.md)
5. [Statistical modelling](statistical-modelling-split.md)
6. [Statistical model](statistical-model-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bayes risk bound for one-nearest-neighbour classification](bayes-risk-bound-for-one-nearest-neighbour-classification.md)
- [Feature-measurable nearest-neighbour tie-breaking](feature-measurable-nearest-neighbour-tie-breaking.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210/2/solution.md)
