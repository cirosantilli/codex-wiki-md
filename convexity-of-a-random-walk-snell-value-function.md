# Convexity of a random-walk Snell value function

↑ **Parent:** [Optimal stopping value function](optimal-stopping-value-function.md)

The [transition operator](transition-operator.md) of an additive [random walk](random-walk.md) preserves [convex functions](convex-function.md): apply their convexity inequality to $x+\xi$ and $y+\xi$, then integrate. The [pointwise maximum of convex functions](pointwise-maximum-of-convex-functions.md) preserves convexity too, so induction proves convexity of the [Snell envelope](snell-envelope.md) Bellman functions. Expectations are allowed to be extended-valued until finiteness is justified. Integrability of rewards on a finite horizon implies finiteness of these functions at every state for $t\geq1$, by [integrability of translated convex random-walk rewards](integrability-of-translated-convex-random-walk-rewards.md) and the bound $W_t(x)\leq\sum_{j=0}^{T-t}\mathbb E[f(x+Z_j)^+]$. At time zero only $X_0=0$ is observed; if $W_0$ is infinite elsewhere, its finite value at zero has a constant convex extension representing the same Snell envelope. Full statewise Bellman recursion at time zero requires an additional translated-integrability hypothesis.

## ↑ Ancestors (9)

1. [Optimal stopping value function](optimal-stopping-value-function.md)
2. [Optimal stopping](optimal-stopping.md)
3. [Snell envelope](snell-envelope.md)
4. [Martingale](martingale-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39/3/c/solution.md)
