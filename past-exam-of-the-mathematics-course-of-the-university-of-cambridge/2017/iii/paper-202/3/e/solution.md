<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**No absolutely continuous probability measure can remove this nonzero drift on the whole half-line.** By the [strong law for Brownian motion](../../../../../../strong-law-for-brownian-motion.md), the event

$$
A=\left\{\lim_{t\to\infty}\frac{B_t}{t}=0\right\}
$$

has $\mathbb P$-probability one. If $\mathbb P^\infty\ll\mathbb P$, [absolute continuity of measures](../../../../../../absolute-continuity-of-measures.md) gives $\mathbb P^\infty(A)=1$. But if $W_t=B_t-\mu t$ is a [Brownian motion](../../../../../../brownian-motion-split.md) under $\mathbb P^\infty$, the same [strong law for Brownian motion](../../../../../../strong-law-for-brownian-motion.md) gives $B_t/t=W_t/t+\mu\to\mu$ with $\mathbb P^\infty$-probability one. Since $\mu>0$, these two limiting events are disjoint, a contradiction.

This is [infinite-horizon singularity of Brownian motion with constant drift](../../../../../../infinite-horizon-singularity-of-brownian-motion-with-constant-drift.md). The finite-horizon densities are consistent on $\mathcal F_t$ but cannot define a globally absolutely continuous measure with the requested property. Indeed,

$$
\boxed{Z_t\longrightarrow0\quad\mathbb P\text{-almost surely},\qquad \mathbb E Z_t=1,}
$$

because $t^{-1}\log Z_t\to-\mu^2/2$. Hence $Z$ lacks [uniform integrability](../../../../../../uniform-integrability.md) on $[0,\infty)$. A drifted law does exist on canonical path space, but it is mutually singular with [Wiener measure](../../../../../../wiener-measure.md) on the infinite-horizon path [sigma-algebra](../../../../../../sigma-algebra.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
