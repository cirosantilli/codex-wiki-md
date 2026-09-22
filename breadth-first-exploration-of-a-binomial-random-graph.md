# Breadth-first exploration of a binomial random graph

↑ **Parent:** [Erdős-Rényi model](erdos-renyi-model.md)

During [Breadth-first search](breadth-first-search.md) of $G(n,p)$ let $U_t$ count unseen [vertices](vertex-graph-theory.md), $A_t$ active [vertices](vertex-graph-theory.md), and $t$ explored [vertices](vertex-graph-theory.md). When $A_{t-1}=0$ start a new unseen root, recorded by $b_t=1$; otherwise $b_t=0$. The newly discovered count is conditionally $\operatorname{Bin}(U_{t-1}-b_t,p)$. Subtract its conditional mean to obtain a [martingale difference](martingale-difference.md) $D_t$. With $q=1-p$, $U_0=n$ and $A_0=0$, iteration gives

$$
A_t=n-t-nq^t+\sum_{j\leq t}q^{t-j+1}b_j+q^t\sum_{j\leq t}q^{-j}D_j.
$$

The last sum is a [martingale](martingale-split.md). Positive $A_t$ over an interval means that the [graph component](component-graph-theory.md) under exploration does not finish there. Independently adding phantom children couples each component exploration below a [binomial branching process](binomial-branching-process.md) with offspring law $\operatorname{Bin}(n,p)$.

## ↑ Ancestors (7)

1. [Erdős-Rényi model](erdos-renyi-model.md)
2. [Random graph](random-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Barely-supercritical largest-component expectation](barely-supercritical-largest-component-expectation.md)
- [Binomial branching process](binomial-branching-process.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/4/ii/solution.md)
