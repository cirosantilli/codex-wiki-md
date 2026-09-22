<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an elementary [previsible process](../../../../../../predictable-process.md) $H=\sum_{j=0}^{r-1}H_j\mathbf1_{(t_j,t_{j+1}]}$, with bounded $\mathcal F_{t_j}$-measurable coefficients, define

$$
(H\cdot M)_t=\sum_j H_j\big(M_{t\wedge t_{j+1}}-M_{t\wedge t_j}\big).
$$

The [Itô isometry](../../../../../../ito-isometry.md) is

$$
\boxed{\mathbb E\big[(H\cdot M)_t^2\big]=\mathbb E\int_0^t H_s^2\,d[M]_s.}
$$

More generally the squared $L^2$ distance between the integrals of $H$ and $K$ is the integral of $(H-K)^2$ on the right. The integral is a zero-starting continuous square-integrable [martingale](../../../../../../martingale-split.md).

Elementary [predictable processes](../../../../../../predictable-process.md) are dense in $L^2(M)$. Given $H$ in this space, choose elementary $H_n$ converging in its norm and define the [Itô integral](../../../../../../ito-integral.md) by the $L^2$ limit of $H_n\cdot M$. The isometry proves that this is independent of the approximating sequence and remains valid for the limit. The [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) bounds the expected squared path supremum of the difference by four times its terminal second moment; hence the convergence also gives a continuous [martingale](../../../../../../martingale-split.md) version, with [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md).

For a [continuous local martingale](../../../../../../continuous-local-martingale.md) $M$ and [locally bounded process](../../../../../../locally-bounded-process.md) $H$ that is [previsible](../../../../../../predictable-process.md), choose increasing [stopping times](../../../../../../stopping-time.md) $\tau_n\uparrow\infty$ such that $M^{\tau_n}$ is L2-bounded, $|H|\le K_n$ up to $\tau_n$, and $\tau_n\le n$. This can be done by combining localizers with first exits of $M$ from bounded intervals and the local bounds of $H$. Then $H\mathbf1_{[0,\tau_n]}$ is in the integrand space for $M^{\tau_n}$. Define the integral on each stopped interval by the preceding construction. The stopping property of elementary integrals, extended by the isometry, makes these definitions agree on overlaps. Pasting gives

$$
\boxed{H\cdot M\text{ as a continuous local martingale, defined consistently on all }[0,\tau_n].}
$$

This is a localization construction; global square integrability of the resulting process is not asserted.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
