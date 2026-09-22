<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose the [utility function](../../../../../../utility-function-split.md) primitive $U(c)=c^{1-R}/(1-R)$. Any other primitive with the same [derivative](../../../../../../derivative.md) differs by a constant $C$; this adds $C/\rho$ to the [value function](../../../../../../value-function.md) and does not alter the policy. Put $p=1-R$ and let $\pi_t$ be the [stock](../../../../../../stock.md) fraction. The [self-financing portfolio](../../../../../../self-financing-portfolio.md) equation, including [consumption](../../../../../../consumption.md) withdrawals, is

$$
\boxed{dw_t=\bigl[rw_t+\pi_tw_t(\mu-r)-c_t\bigr]dt+\sigma\pi_tw_t\,dW_t.}
$$

For a time-independent infinite-horizon [value function](../../../../../../value-function.md) $V$, the [Hamilton-Jacobi-Bellman equation](../../../../../../hamilton-jacobi-bellman-equation.md) is

$$
\rho V(w)=\sup_{c>0,\,\pi}\left\{\frac{c^p}{p}+\bigl[rw+\pi w(\mu-r)-c\bigr]V'(w)+\frac12\sigma^2\pi^2w^2V''(w)\right\}.
$$

Scaling initial [portfolio wealth](../../../../../../portfolio-wealth.md) and all [consumption](../../../../../../consumption.md) rates by the same positive number preserves admissibility and scales [utility function](../../../../../../utility-function-split.md) by its $p$th power. This [homogeneity](../../../../../../homogeneity.md) gives $V(w)=Kw^p/p$. In particular,

$$
V'(w)=Kw^{-R},\qquad V''(w)=-RKw^{-R-1}.
$$

The [consumption](../../../../../../consumption.md) [first-order condition](../../../../../../first-order-optimality-condition.md) $c^{-R}=V'(w)$ and [stock](../../../../../../stock.md) [first-order condition](../../../../../../first-order-optimality-condition.md) $w(\mu-r)V'(w)+\sigma^2\pi w^2V''(w)=0$ give

$$
\pi_M=\frac{\mu-r}{R\sigma^2},\qquad c=K^{-1/R}w.
$$

The [second derivatives](../../../../../../second-derivative.md) of the optimized expressions are negative, so these are their global maximizers. Writing $\gamma_M=K^{-1/R}$ and substituting into the [Hamilton-Jacobi-Bellman equation](../../../../../../hamilton-jacobi-bellman-equation.md) gives

$$
\rho=R\gamma_M+(1-R)\left(r+\frac{(\mu-r)^2}{2R\sigma^2}\right).
$$

Therefore

$$
\boxed{\pi_M=\frac{\mu-r}{R\sigma^2},\qquad
\gamma_M=\frac{\rho+(R-1)\left(r+\frac{(\mu-r)^2}{2R\sigma^2}\right)}{R},\qquad
c_t^*=\gamma_Mw_t.}
$$

The given inequality is precisely $\gamma_M>0$, so the [Merton consumption-investment problem](../../../../../../merton-consumption-investment-problem.md) value is $V(w)=\gamma_M^{-R}w^{1-R}/(1-R)$. This derives the requested policy; no additional verification argument is needed here.

## ↑ Ancestors (11)

1. [I](../i.md)
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
