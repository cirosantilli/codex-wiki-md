# Barely-supercritical largest-component expectation

↑ **Parent:** [Giant component](giant-component.md)

Suppose $\varepsilon=o(1)$ and $\varepsilon\geq n^{-1/6}$. The [breadth-first exploration of a binomial random graph](breadth-first-exploration-of-a-binomial-random-graph.md) has deterministic drift $F(t)=\varepsilon t-t^2/(2n)+O(\varepsilon^3n+\varepsilon)$ up to $3\varepsilon n$ steps. Its weighted [martingale](martingale-split.md) has [variance](variance-split.md) $O(\varepsilon n)$. For $h=\sqrt\varepsilon+(n\varepsilon^3)^{-1/8}$, the [Doob L2 maximal inequality](doob-l2-maximal-inequality.md) makes its maximum smaller than $h\varepsilon^2n/6$ [with high probability](with-high-probability.md). Then $A_t>0$ throughout $[h\varepsilon n,(2-h)\varepsilon n]$, giving a [graph component](component-graph-theory.md) of order $(2-o(1))\varepsilon n$.

For the upper expectation bound, let $K=\lceil\varepsilon^{-3}\rceil$. The dominating [binomial branching process](binomial-branching-process.md) has [branching survival probability](survival-probability-of-a-branching-process.md) $(2+o(1))\varepsilon$ by the [binomial branching survival correction](binomial-branching-survival-correction.md). Its [branching process conditioned on extinction](branching-process-conditioned-on-extinction.md) has mean $1-\varepsilon+O(\varepsilon^2+\varepsilon/n)$ and total-progeny [expected value](expected-value.md) $O(1/\varepsilon)$. Therefore $\mathbb EN_{\geq K}\leq n\rho+O(n/(\varepsilon K))$. Since $L_1\leq K+N_{\geq K}$ and $K=o(\varepsilon n)$, this yields the matching upper bound. Controlling rare large components is necessary to conclude an [expected value](expected-value.md) asymptotic from a typical-size statement.

## ↑ Ancestors (7)

1. [Giant component](giant-component.md)
2. [Random graph](random-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/4/ii/solution.md)
