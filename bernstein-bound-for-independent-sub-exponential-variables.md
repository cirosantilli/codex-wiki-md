# Bernstein bound for independent sub-exponential variables

↑ **Parent:** [Bernstein inequalities (probability theory)](bernstein-inequalities-probability-theory.md)

Suppose independent centered [sub-exponential random variables](subexponential-distribution-light-tailed.md) satisfy $\log\mathbb E e^{\lambda X_i}\leq v_i\lambda^2/(2(1-b|\lambda|))$ for $|\lambda|<1/b$, and put $v=\sum_iv_i$. Independence adds the log [moment-generating functions](moment-generating-function.md). The [Chernoff bound](chernoff-bound.md) with $\lambda=t/(v+bt)$ gives the displayed two-sided tail. If each variable has common scale $K$, one may take $v_i\leq CK^2$ and $b\leq CK$, giving $\mathbb P(|n^{-1}\sum_iX_i|>t)\leq2e^{-c n\min\{t^2/K^2,t/K\}}$. This form of [Bernstein's inequality](bernstein-inequalities-probability-theory.md) allows unbounded variables with factorial moment control, including the [centered square of a sub-Gaussian random variable](centered-square-of-a-sub-gaussian-random-variable.md).

## ↑ Ancestors (9)

1. [Bernstein inequalities (probability theory)](bernstein-inequalities-probability-theory.md)
2. [Sub-Gamma random variable in the right tail](sub-gamma-random-variable-in-the-right-tail.md)
3. [Concentration inequality](concentration-inequality.md)
4. [Probability inequality](probability-inequality-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Centered square of a sub-Gaussian random variable](centered-square-of-a-sub-gaussian-random-variable.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/2/b/solution.md)
