# Second-order boundary expansion for local constant regression

↑ **Parent:** [Boundary bias of local constant regression](boundary-bias-of-local-constant-regression.md)

For fixed $\alpha\in[0,1)$, design $x_i=i/n$, $m\in C^2[0,1]$, a nonzero nonnegative symmetric piecewise $C^1$ [regression kernel](kernel-for-nonparametric-regression.md) supported on $[-1,1]$, and $h\to0$, $nh^2\to\infty$, write $\mu_{r,\alpha}=\int_{-\alpha}^1u^rK(u)\,du$ and $\beta_r=\mu_{r,\alpha}/\mu_{0,\alpha}$. On the rescaled grid of spacing $1/(nh)$, the [Riemann sum](riemann-sum.md) error for $u^rK(u)$ is $O((nh)^{-1})$, by [bounded variation](total-variation-of-a-function.md). The normalized first and second local moments are therefore $h\beta_1+O(n^{-1})$ and $h^2\beta_2+O(h/n)$. A uniform second-order [Taylor expansion](taylor-expansion.md) gives the displayed [bias of an estimator](bias-of-an-estimator.md), since $n^{-1}=o(h^2)$. Equivalently it is $h\beta_1m'(0)+h^2(\alpha\beta_1+\beta_2/2)m''(0)+o(h^2)$. The first-order term explains the generic boundary bias of a [local constant estimator](nadaraya-watson-estimator.md).

## ↑ Ancestors (10)

1. [Boundary bias of local constant regression](boundary-bias-of-local-constant-regression.md)
2. [Nadaraya–Watson estimator](nadaraya-watson-estimator.md)
3. [Local polynomial regression](local-polynomial-regression.md)
4. [Nonparametric regression](nonparametric-regression.md)
5. [Nonparametric statistics](nonparametric-statistics-split.md)
6. [Statistical inference](statistical-inference-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/2/solution.md)
