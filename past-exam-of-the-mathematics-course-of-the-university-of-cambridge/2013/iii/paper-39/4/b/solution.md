<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The first-contact time $\tau_*\le T$ is a [stopping time](../../../../../../stopping-time.md): the event $\{\tau_*\le t\}$ is the finite union of events $\{U_s=Y_s\}$ for $s\le t$. It is finite because $U_T=Y_T$. On $\{\tau_*>t\}$ we have $U_t>Y_t$, so the maximum defining the [Snell envelope](../../../../../../snell-envelope.md) selects continuation and

$$
U_t=\mathbb E(U_{t+1}\mid\mathcal F_t).
$$

The stopped process $U_{t\wedge\tau_*}$ is therefore a [martingale](../../../../../../martingale-split.md): before stopping its conditional increment is zero and after stopping its increment vanishes. Applying the stopped-sum argument with zero conditional increments gives

$$
\boxed{U_0=\mathbb E U_{\tau_*}=\mathbb E Y_{\tau_*}.}
$$

The upper bound from part (a) now proves that first contact is an [optimal stopping time](../../../../../../optimal-stopping-time.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
