# Clipped acceptance reweighting identity

↑ **Parent:** [Rejection sampling](rejection-sampling.md)

Draw proposals with [probability density function](probability-density-function.md) or [probability mass function](probability-mass-function.md) $q$, independently draw $U$ from the [uniform distribution](continuous-uniform-distribution.md) on $(0,1)$, and repeat until $U\leq h(Y)$ for a nonnegative threshold $h$. The actual acceptance [probability](probability.md) given $Y=y$ is $a(y)=\min(1,h(y))$. If $A=\mathbb E_q[a(Y)]>0$, the returned [probability distribution](probability-distribution-split.md) has density or mass $q(y)a(y)/A$. Indeed the joint law of a proposal and acceptance has density or mass $q(y)a(y)$, and conditioning on acceptance divides by $A$. Summing over failed trials gives the same law and expected trial count $1/A$. Thresholds exceeding one cannot be used as unbounded reweighting factors.

## ↑ Ancestors (6)

1. [Rejection sampling](rejection-sampling.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2021/2/b/i/solution.md)
