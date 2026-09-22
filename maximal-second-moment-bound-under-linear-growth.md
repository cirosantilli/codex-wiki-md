# Maximal second-moment bound under linear growth

↑ **Parent:** [Linear growth condition for an SDE](linear-growth-condition-for-an-sde.md)

For $dX=\sigma(X)dB+b(X)dt$, $X_0=0$, and $\sigma^2+b^2\leq A(1+X^2)$, the [Doob L2 maximal inequality](doob-l2-maximal-inequality.md) and the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) imply, for $t\leq1$, $F(t)\leq8A\int_0^t(1+F(s))ds$, where $F(t)=\mathbb E\sup_{s\leq t}|X_s|^2$. The [Gronwall inequality](gronwall-inequality.md) yields $F(t)\leq e^{8At}-1$. Apply the calculation first to stopped paths; truncating [locally Lipschitz functions](locally-lipschitz-function.md) and using this uniform bound gives exit probabilities at most $(e^{8A}-1)/n^2$, proving nonexplosion on the unit time interval.

## ↑ Ancestors (11)

1. [Linear growth condition for an SDE](linear-growth-condition-for-an-sde.md)
2. [Existence and pathwise uniqueness theorem for a stochastic differential equation](existence-and-pathwise-uniqueness-theorem-for-a-stochastic-differential-equation.md)
3. [Maximal local solution of a stochastic differential equation](maximal-local-solution-of-a-stochastic-differential-equation.md)
4. [Stochastic differential equation](stochastic-differential-equation.md)
5. [Stochastic calculus](stochastic-calculus-split.md)
6. [Stochastic process](stochastic-process-split.md)
7. [Probability theory](probability-theory-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24/4/solution.md)
