<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $M_t=\int_0^tH_s\,dB_s$ and $A_t=\int_0^tH_s^2ds=[M]_t$. The assumed path properties make $A$ continuous, strictly increasing and unbounded. Therefore $T$ is a finite [stopping time](../../../../../../stopping-time.md) and $A_T=\sigma^2$, even though its definition uses a strict inequality.

For $u\in\mathbb R$, the [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
E_t=\exp\left(iuM_{t\wedge T}+\frac{u^2}{2}A_{t\wedge T}\right),\qquad
dE_t=iuE_t\,dM_{t\wedge T}.
$$

Its real and imaginary parts are [local martingales](../../../../../../local-martingale.md), and $|E_t|\le e^{u^2\sigma^2/2}$. Thus $E$ is a bounded true [martingale](../../../../../../martingale-split.md). Continuity of $M$, finiteness of $T$, and [dominated convergence](../../../../../../dominated-convergence-theorem.md) yield $\mathbb E E_T=1$. Rearranging gives

$$
\mathbb E e^{iuM_T}=e^{-u^2\sigma^2/2}.
$$

The [characteristic function](../../../../../../characteristic-function.md) uniquely identifies the distribution, proving the [Gaussian terminal value at a deterministic bracket level](../../../../../../gaussian-terminal-value-at-a-deterministic-bracket-level.md):

$$
\boxed{\int_0^T H_s\,dB_s\sim N(0,\sigma^2).}
$$

This proof does not use the time-change theorem that the later part asks us to prove.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
