<h1 id="26j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [Inhomogeneous Poisson process](../../../../../../inhomogeneous-poisson-process.md) with deterministic, nonnegative locally integrable rate $\lambda(t)$ is a counting process $N$ with $N(0)=0$, independent increments, and increment distribution

$$
N(t)-N(s)\sim\operatorname{Poisson}\left(\int_s^t\lambda(u)\,du\right),\quad0\leq s<t.
$$

Equivalently, for continuous rates it is a simple counting process with independent increments and infinitesimal probabilities $\mathbb P(N(t+h)-N(t)=1)=\lambda(t)h+o(h)$ and $\mathbb P(N(t+h)-N(t)\geq2)=o(h)$. For merely locally integrable rates use the integrated-rate formulation, which avoids a pointwise regularity assumption.

$$
\boxed{N(t)-N(s)\sim\operatorname{Poisson}\!\left(\int_s^t\lambda(u)\,du\right).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [26J](../../26j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
