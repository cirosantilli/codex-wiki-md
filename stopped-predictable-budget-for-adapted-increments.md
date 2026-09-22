# Stopped predictable budget for adapted increments

↑ **Parent:** [Stopped process](stopped-process.md)

For finite nonnegative [adapted processes](adapted-process.md) $Y_j$, set $\tau_a=\inf\{n:\sum_{j\leq n}Y_j>a\}$ and $U_n=\sum_{j<n}Y_j$. Stopping this one-step-lagged sum gives $A_n=a-U_{n\wedge\tau_a}\in[0,a]$, with $A_{n+1}-A_n=-Y_n\mathbf1_{\{\tau_a>n\}}$. The latter is nonpositive and [measurable](measurability.md) at time $n$, so $A$ is a nonnegative [supermartingale](supermartingale.md). The overshooting increment is excluded, which is essential to nonnegativity.

## ↑ Ancestors (8)

1. [Stopped process](stopped-process.md)
2. [Stopping time](stopping-time.md)
3. [Martingale](martingale-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28/3/b/solution.md)
- [Supermartingale convergence with summable adapted drift](supermartingale-convergence-with-summable-adapted-drift.md)
