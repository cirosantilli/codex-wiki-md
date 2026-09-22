<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The correct [quadratic variation of a stochastic integral](../../../../../../quadratic-variation-of-a-stochastic-integral.md) identity is

$$
\boxed{[H\cdot M]_t=\int_0^t H_s^2\,d[M]_s=(H^2\cdot[M])_t.}
$$

The brackets around the final integrator are missing in the PDF. Without them the assertion is false: for $H=1$ and $M$ [Brownian motion](../../../../../../brownian-motion-split.md), the left side is $t$ while the printed right side is $B_t$.

For elementary [predictable](../../../../../../predictable-process.md) $H$, the integral is obtained by scaling each [martingale](../../../../../../martingale-split.md) increment by its known coefficient. [Quadratic variation](../../../../../../quadratic-variation.md) on each interval is therefore scaled by the square of that coefficient, giving the displayed formula. To pass to a general $L^2(M)$ integrand on $[0,T]$, take elementary $H_n\to H$ in the integrand norm and put $N_n=H_n\cdot M$, $N=H\cdot M$. The [Itô isometry](../../../../../../ito-isometry.md) gives $\mathbb E(N_n-N)_T^2\to0$, hence $\mathbb E[N_n-N]_T\to0$. The bracket Cauchy-Schwarz bound

$$
|[N,N_n-N]_t|\le[N]_T^{1/2}[N_n-N]_T^{1/2}\qquad(t\le T)
$$

and polarization show that $[N_n]\to[N]$ uniformly in probability. On the other side, Cauchy-Schwarz for the [quadratic-variation measure](../../../../../../quadratic-variation-measure.md) gives

$$
\mathbb E\int_0^T|H_n^2-H^2|\,d[M]\le\|H_n-H\|_{L^2(M;T)}\big(\|H_n\|_{L^2(M;T)}+\|H\|_{L^2(M;T)}\big)\longrightarrow0.
$$

Taking limits proves the formula in the square-integrable case. Stopping and pasting as in part b proves it for locally bounded [predictable](../../../../../../predictable-process.md) integrands and [continuous local martingales](../../../../../../continuous-local-martingale.md).

## ↑ Ancestors (11)

1. [D](../d.md)
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
