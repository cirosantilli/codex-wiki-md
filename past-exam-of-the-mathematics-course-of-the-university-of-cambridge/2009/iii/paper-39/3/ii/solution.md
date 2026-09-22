<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the positive constant

$$
k=\rho+(R-1)\left(\alpha-\frac12R\sigma^2\right).
$$

Since $S=\delta/k$, the [stock](../../../../../../stock.md) price has capital-appreciation dynamics $dS/S=\alpha dt+\sigma dW$. But each share also pays the flow $\delta=kS$. Its [dividend-inclusive portfolio return](../../../../../../dividend-inclusive-portfolio-return.md) therefore has [drift](../../../../../../drift-coefficient.md)

$$
\mu_{\mathrm{total}}=\alpha+k.
$$

This is the [drift](../../../../../../drift-coefficient.md) to use in the [Merton consumption-investment problem](../../../../../../merton-consumption-investment-problem.md); using only capital appreciation would omit an actual source of [portfolio wealth](../../../../../../portfolio-wealth.md).

At the proposed bank rate,

$$
\mu_{\mathrm{total}}-r^*
=\alpha+k-\left[\rho+R\alpha-\frac12(1+R)R\sigma^2\right]
=R\sigma^2.
$$

Thus the optimal [stock](../../../../../../stock.md) fraction from part (i) is

$$
\boxed{\pi_M=1.}
$$

Moreover,

$$
r^*+\frac{(\mu_{\mathrm{total}}-r^*)^2}{2R\sigma^2}
=\rho+R\alpha-\frac12R^2\sigma^2.
$$

Substituting this into the optimal [consumption](../../../../../../consumption.md) coefficient yields

$$
\gamma_M=\frac{\rho+(R-1)\left(\rho+R\alpha-\frac12R^2\sigma^2\right)}{R}
=\rho+(R-1)\left(\alpha-\frac12R\sigma^2\right)=k>0.
$$

Hence the finite-value condition in part (i) is automatically satisfied.

The agent's endowment of the single productive share has [portfolio wealth](../../../../../../portfolio-wealth.md) $w=S$. Investing fraction one in the [stock](../../../../../../stock.md) means holding $w/S=1$ share, leaving $w-S=0$ in the [bank account](../../../../../../bank-account.md). The optimal [consumption](../../../../../../consumption.md) rate is

$$
\boxed{c_t=\gamma_Mw_t=kS_t=\delta_t.}
$$

This policy also satisfies the [self-financing portfolio](../../../../../../self-financing-portfolio.md) equation: with one share and no bank balance,

$$
dw_t=dS_t+\delta_tdt-c_tdt=dS_t.
$$

Thus $w_t=S_t$ remains valid at all times. **The agent holds the entire one-share supply, has zero net borrowing or lending, and consumes exactly the supplied goods.** The [stock](../../../../../../stock.md), bank-account and consumption-good markets all clear.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
