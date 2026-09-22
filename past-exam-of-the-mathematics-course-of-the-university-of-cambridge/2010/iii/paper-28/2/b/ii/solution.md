<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $(B_t)_{0\leq t\leq1}$ be standard [Brownian motion](../../../../../../../brownian-motion-split.md) with its continuous version, and define

$$
\boxed{Z_t=B_t-tB_1.}
$$

Every finite vector is a linear transform of a Gaussian Brownian vector, so $Z$ is a centred [Gaussian process](../../../../../../../gaussian-process.md). Using $\mathbb E[B_sB_t]=\min(s,t)$,

$$
\mathbb E[Z_sZ_t]
=\min(s,t)-t\,s-s\,t+st
=\min(s,t)-st.
$$

For $s\leq t$, this is $s(1-t)$, the prescribed [Brownian bridge covariance kernel](../../../../../../../brownian-bridge-covariance-kernel.md). Its paths are continuous on the probability-one event of Brownian continuity, because $t\mapsto tB_1$ is continuous on every sample. The construction also gives $Z_0=Z_1=0$. Thus it realizes a [Brownian bridge](../../../../../../../brownian-bridge.md) with [almost surely](../../../../../../../almost-sure-convergence.md) continuous paths, and part (i) identifies its process law.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
