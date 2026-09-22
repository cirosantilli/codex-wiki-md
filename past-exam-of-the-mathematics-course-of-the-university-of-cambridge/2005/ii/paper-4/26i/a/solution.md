<h1 id="26i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The embedded [birth-death chain](../../../../../../birth-death-chain.md) has upward [probability](../../../../../../probability.md) $p_k=(k+2)/(2(k+1))$ and downward [probability](../../../../../../probability.md) $q_k=k/(2(k+1))$. To calculate a return [probability](../../../../../../probability.md), solve the [harmonic](../../../../../../harmonic-function.md) difference equation on $\{0,\ldots,m\}$ with boundary values one at zero and zero at $m$. Successive differences have ratio $q_k/p_k=k/(k+2)$, so their weights are

$$
r_0=1,\qquad r_j=\prod_{k=1}^j\frac{k}{k+2}
=\frac2{(j+1)(j+2)}.
$$

Their total infinite sum is $2$. Letting $m\to\infty$ gives the [probability](../../../../../../probability.md) of ever hitting zero from $k$:

$$
h_k=\frac{\sum_{j=k}^\infty r_j}{\sum_{j=0}^\infty r_j}
=\boxed{\frac1{k+1}}.
$$

In particular the chain leaves zero to one and returns with [probability](../../../../../../probability.md) $1/2<1$, so it is **transient**. This finite-interval calculation selects the minimal nonnegative hitting-probability solution, rather than merely observing that $h_k$ is [harmonic](../../../../../../harmonic-function.md).

The continuous-time chain has the same embedded transitions and constant total exit rate $2/3$, so it is nonexplosive and has exactly the same return events. It too is **transient**, neither [positive recurrent](../../../../../../positive-recurrent-markov-chain.md) nor [null recurrent](../../../../../../null-recurrent-state.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26I](../../26i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
