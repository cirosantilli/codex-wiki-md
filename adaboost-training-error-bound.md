# AdaBoost training error bound

↑ **Parent:** [Exponential-loss derivation of AdaBoost](exponential-loss-derivation-of-adaboost.md)

For [AdaBoost](adaboost.md) with initial uniform weights, labels and base predictions in $\{-1,1\}$, and edges $\gamma_m=1/2-\epsilon_m>0$, the training [exponential classification risk](exponential-classification-risk.md) equals the product of stage normalizers. A wrongly classified point has exponential loss at least one, so empirical classification error is bounded by this product. The final inequality uses $\sqrt{1-4\gamma_m^2}\le e^{-2\gamma_m^2}$. The result concerns training error, not a guarantee against overfitting or mislabeled observations.

// Target: probability-and-statistics.bigb

## ↑ Ancestors (7)

1. [Exponential-loss derivation of AdaBoost](exponential-loss-derivation-of-adaboost.md)
2. [AdaBoost](adaboost.md)
3. [Statistical learning theory](statistical-learning-theory.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45/3/b/solution.md)
- [Weak learner](weak-learner.md)
