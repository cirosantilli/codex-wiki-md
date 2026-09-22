# Classification-tree deviance

↑ **Parent:** [Classification tree](classification-tree.md)

Maximizing a node's multinomial likelihood gives class probabilities $\widehat p_{tk}=n_{tk}/n_t$. Twice the negative maximized log-likelihood relative to perfect classification is the displayed deviance, with $0\log0=0$. It equals twice the node size times its [Shannon entropy](information-entropy.md). A split is chosen by maximizing $D(t)-D(t_L)-D(t_R)$, and tree deviance is the sum over terminal nodes. The training misclassification count is instead $\sum_t(n_t-\max_kn_{tk})$; the two criteria are different.

## ↑ Ancestors (9)

1. [Classification tree](classification-tree.md)
2. [Classification in statistical learning](classification-in-statistical-learning.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Classification tree](classification-tree.md)
- [Misclassification rate](misclassification-rate.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-39/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46/3/solution.md)
