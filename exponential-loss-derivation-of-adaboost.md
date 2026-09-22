# Exponential-loss derivation of AdaBoost

↑ **Parent:** [AdaBoost](adaboost.md)

At score $F$, the [exponential classification risk](exponential-classification-risk.md) weights observation $i$ proportionally to $e^{-y_iF(x_i)}$. A stage $\alpha G$ multiplies this weight by $e^{-\alpha y_iG(x_i)}$. For weighted error $\epsilon$, the loss multiplier is $(1-\epsilon)e^{-\alpha}+\epsilon e^\alpha$, minimized at the displayed value. Its minimum is $2\sqrt{\epsilon(1-\epsilon)}$. Thus errors gain weight relative to correct observations in the next stage.

// Target: foundations-of-mathematics.bigb

**Table of contents**

- [AdaBoost training error bound](adaboost-training-error-bound.md)

## ↑ Ancestors (6)

1. [AdaBoost](adaboost.md)
2. [Statistical learning theory](statistical-learning-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45/3/b/solution.md)
