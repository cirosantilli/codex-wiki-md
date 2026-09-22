# Self-similar Gaussian workload rate

↑ **Parent:** [Sublinear path space for fluid queues](sublinear-path-space-for-fluid-queues.md)

Let a centered [Gaussian process](gaussian-process.md) $Z$ satisfy $Z(a\,\cdot)\overset d=a^H Z$ with $0<H<1$, and suppose $Z/\sqrt L$ has a [large deviation principle](large-deviation-principle.md) in the [sublinear path space for fluid queues](sublinear-path-space-for-fluid-queues.md), with speed $L$ and [good rate function](good-rate-function.md) $I$. For $\delta,\sigma>0$, put $r=\sup_{t\geq0}(\sigma Z(t)-\delta t)$ and $\kappa=2(1-H)$. Self-similarity gives $Z(N\,\cdot)/N\overset d=Z/\sqrt{N^\kappa}$. Time substitution and the [contraction principle for large deviations](contraction-principle-for-large-deviations.md) therefore give an LDP for $r/N$ with speed $N^\kappa$ and

$$
J(q)=\inf\{I(f):\sup_{t\geq0}(\sigma f(t)-\delta t)=q\}.
$$

The same family $r/(aN)$ has [rate function](rate-function.md) $J(aq)$ by contraction, and $a^\kappa J(q)$ by replacing $N$ with $aN$ and expressing the speed again as $N^\kappa$. Uniqueness of a [rate function](rate-function.md) gives $J(aq)=a^\kappa J(q)$, hence $J(q)=q^\kappa J(1)$ for $q>0$, with $J(0)=0$.

## ↑ Ancestors (8)

1. [Sublinear path space for fluid queues](sublinear-path-space-for-fluid-queues.md)
2. [Stochastic network](stochastic-network.md)
3. [Queueing theory](queueing-theory-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/3/c/solution.md)
