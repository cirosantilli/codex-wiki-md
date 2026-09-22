# Exponential classification risk

↑ **Parent:** [AdaBoost](adaboost.md)

For labels $Y\in\{-1,1\}$ and a real-valued score $f$, the exponential loss is $\phi(Yf(X))=e^{-Yf(X)}$. Its population and empirical risks are

$$
R_\phi(f)=\mathbb E[e^{-Yf(X)}],
\qquad
\widehat R_\phi(f)=\frac1n\sum_{i=1}^ne^{-Y_if(X_i)}.
$$

## ↑ Ancestors (6)

1. [AdaBoost](adaboost.md)
2. [Statistical learning theory](statistical-learning-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [AdaBoost training error bound](adaboost-training-error-bound.md)
- [Exponential-loss derivation of AdaBoost](exponential-loss-derivation-of-adaboost.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/30j/c/solution.md)
