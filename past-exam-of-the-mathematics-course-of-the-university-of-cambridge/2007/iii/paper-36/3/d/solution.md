<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Interpret the otherwise undefined $b_k(t)$ here as the moment $\beta_k(t)$ defined above. For $k=1$, the process is $B_t$, and for $k=2$ it is $B_t^2-t$; both are [martingales](../../../../../../martingale-split.md).

For $k\ge3$, the [Itô formula](../../../../../../ito-s-lemma.md) and the derivative of the [Brownian moment recursion](../../../../../../brownian-moment-recursion.md) yield

$$
d\big(B_t^k-\beta_k(t)\big)=kB_t^{k-1}\,dB_t+\frac{k(k-1)}2\big(B_t^{k-2}-\beta_{k-2}(t)\big)\,dt.
$$

The [stochastic integral](../../../../../../stochastic-integral.md) is a true [martingale](../../../../../../martingale-split.md) on finite horizons, since the required $2k-2$ moment is integrable in time. The continuous finite-variation term is not identically zero. If it were, its continuous derivative would vanish at every time, whereas at a fixed $t>0$, the nondegenerate Gaussian $B_t$ does not almost surely satisfy the polynomial equation $B_t^{k-2}=\beta_{k-2}(t)$. Uniqueness of [continuous semimartingale](../../../../../../continuous-semimartingale.md) decomposition therefore rules out even the [local martingale](../../../../../../local-martingale.md) property. Hence

$$
\boxed{B_t^k-\beta_k(t)\text{ is a martingale precisely for }k=1,2.}
$$

For example $\mathbb E(B_t^3\mid\mathcal F_s)=B_s^3+3(t-s)B_s$, so merely subtracting its zero expectation cannot make the cubic power a [martingale](../../../../../../martingale-split.md). The [centered Brownian powers need not be martingales](../../../../../../centered-brownian-powers-need-not-be-martingales.md) distinction is resolved by subtracting the random drift compensator $k(k-1)\int_0^tB_s^{k-2}ds/2$ instead of the deterministic mean.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
