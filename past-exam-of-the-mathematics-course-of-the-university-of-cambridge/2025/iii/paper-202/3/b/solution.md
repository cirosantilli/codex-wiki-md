<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The $d$-dimensional [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) says that a continuous local martingale $X$ with $X_0=0$ is a standard $d$-dimensional [Brownian motion](../../../../../../brownian-motion-split.md) exactly when

$$
[X^i,X^j]_t=\delta_{ij}t
$$

for all $i,j$ and $t$.

One direction follows directly from independent Gaussian increments. Conversely, fix $\theta\in\mathbb R^d$. Applying [Itô formula](../../../../../../ito-s-lemma.md) and the bracket assumption shows that

$$
Z_t=\exp\left(i\theta\mathbin\cdot X_t+\frac12|\theta|^2t\right)
$$

is a complex local martingale. After stopping $X$ on leaving large balls it is bounded, so optional sampling and then dominated convergence give, for $s<t$,

$$
\mathbb E\left[e^{i\theta\cdot(X_t-X_s)}\mid\mathcal F_s\right]
=e^{-\frac12|\theta|^2(t-s)}.
$$

This is the [characteristic function](../../../../../../characteristic-function.md) of $N(0,(t-s)I_d)$ and is deterministic. Thus each increment is Gaussian with the required covariance and independent of the past. Together with continuity, these are precisely the defining properties of standard $d$-dimensional Brownian motion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
