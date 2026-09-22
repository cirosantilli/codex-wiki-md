# Elliptical potential bound

↑ **Parent:** [Multi-armed bandit](multi-armed-bandit.md)

Let $V_t=V_{t-1}+x_tx_t^T$ with [positive-definite matrix](positive-definite-matrix.md) $V_0$, and suppose $u_t=x_t^TV_{t-1}^{-1}x_t\leq1$. The [matrix determinant lemma](matrix-determinant-lemma.md) gives $\det V_t/\det V_{t-1}=1+u_t$. Since $2\log(1+u)-u$ has nonnegative derivative $(1-u)/(1+u)$ for $0\leq u\leq1$, summation proves the displayed bound. In particular, $V_0=\lambda I$, $\lambda\geq1$, and $\|x_t\|_2\leq1$ ensure $u_t\leq1$. Without that restriction a general form is $\sum_t\min\{1,u_t\}\leq2\log(\det V_n/\det V_0)$: for $u\geq1$, $2\log(1+u)\geq2\log2\geq1$. The bound connects widths of [confidence ellipsoids](confidence-ellipsoid.md) to growth of a [determinant](determinant.md).

## ↑ Ancestors (9)

1. [Multi-armed bandit](multi-armed-bandit.md)
2. [Online learning](online-learning.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algorithmic-foundations-of-learning-course-of-the-university-of-oxford/2025/2/a/i/solution.md)
