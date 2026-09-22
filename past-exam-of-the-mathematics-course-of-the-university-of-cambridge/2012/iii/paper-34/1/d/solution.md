<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the shifted filtration $\mathcal G_s=\mathcal F_{T+s}$. Each $T+s$ is a [stopping time](../../../../../../stopping-time.md), and the [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) implies that $M_s^{(T)}=M_{T+s}-M_T$ is a $\mathcal G_s$-martingale. It is $L^2$-bounded, for example by $\mathbb E|M_{T+s}-M_T|^2\leq4\mathbb E M_\infty^2$. Its [quadratic variation](../../../../../../quadratic-variation.md) is $[M^{(T)}]_s=[M]_{T+s}-[M]_T$. The shifted process $H_{T+s}$ is continuous and $\mathcal G_s$-adapted, hence [predictable](../../../../../../predictable-process.md). Its boundedness and the integrability of the bracket make the right-hand [stochastic integral](../../../../../../stochastic-integral.md) well-defined in $L^2$.

For a deterministic partition $0=s_0<\cdots<s_r=t$, use left-endpoint coefficients $H_{T+s_j}$. Both integrals have the same approximating sum

$$
\sum_{j=0}^{r-1}H_{T+s_j}(M_{T+s_{j+1}}-M_{T+s_j}).
$$

On the original clock this is the integral of the simple process on the stopping-time intervals $(T+s_j,T+s_{j+1}]$; on the shifted clock it is a deterministic-partition integral. As the mesh tends to zero, continuity of $H$ gives pathwise uniform approximation on the random compact interval $[T,T+t]$. The [Itô isometry](../../../../../../ito-isometry.md) and domination by a constant times the integrable $[M]_\infty$ give $L^2$ convergence of both sums. Thus [stopping-time shift of a stochastic integral](../../../../../../stopping-time-shift-of-a-stochastic-integral.md) yields

$$
\boxed{\int_T^{T+t}H_s\,dM_s=\int_0^tH_{T+s}\,dM_s^{(T)}.}
$$

The left integral includes increments strictly after $T$, so no jump at the starting time is added.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
