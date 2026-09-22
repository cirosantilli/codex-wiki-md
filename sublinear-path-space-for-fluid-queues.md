# Sublinear path space for fluid queues

↑ **Parent:** [Stochastic network](stochastic-network.md)

The useful infinite-horizon path space for a stable [queue](queue-queueing-theory.md) is

$$
\mathcal C_0=\{f\in C([0,\infty)):f(0)=0,\ f(t)/(1+t)\to0\},\qquad
\|f\|_{\rm sl}=\sup_{t\geq0}|f(t)|/(1+t).
$$

For $\delta,\sigma>0$, the workload functional $R(f)=\sup_{t\geq0}(\sigma f(t)-\delta t)$ is finite and [continuous](continuous-function.md). Fix $f$, and choose $T\geq1$ so that $|\sigma f(t)|\leq\delta t/4$ for $t\geq T$. If $\|g-f\|_{\rm sl}<\delta/(4\sigma)$, then $\sigma g(t)-\delta t<0$ for $t\geq T$. Both suprema can thus be taken over $[0,T]$, where

$$
|R(g)-R(f)|\leq\sigma(1+T)\|g-f\|_{\rm sl}.
$$

Uniform convergence on bounded time intervals alone does not give this continuity: a pulse escaping to later times can produce a large workload while tending locally to zero.

**Table of contents**

- [Weighted cumulative-input topology for a slotted queue](weighted-cumulative-input-topology-for-a-slotted-queue.md)
- [Self-similar Gaussian workload rate](self-similar-gaussian-workload-rate.md)

## ↑ Ancestors (7)

1. [Stochastic network](stochastic-network.md)
2. [Queueing theory](queueing-theory-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/3/b/solution.md)
- [Self-similar Gaussian workload rate](self-similar-gaussian-workload-rate.md)
