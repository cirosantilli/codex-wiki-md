<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume $f\in C^{1,2}$ on positive prices before maturity and the usual local trading integrability. If its value is held in [stock](../../../../../stock.md) units $\delta_t$ and bank units $\beta_t$, then

$$
f(S_t,t)=\delta_t S_t+\beta_t B_t,\qquad
 df=\delta_t\,dS_t+\beta_t\,dB_t
$$

for a [self-financing portfolio](../../../../../self-financing-portfolio.md). The [Itô formula](../../../../../ito-s-lemma.md) diffusion coefficient is $\sigma S_tf_x$, so $\sigma S_t>0$ forces $\delta_t=f_x(S_t,t)$ and $\beta_tB_t=f-S_tf_x$. Equating drifts yields

$$
f_t+\alpha xf_x+\frac12\sigma^2x^2f_{xx}
=\alpha xf_x+\rho(f-xf_x).
$$

The physical drift cancels, giving the [Black-Scholes equation](../../../../../black-scholes-equation.md)

$$
\boxed{f_t+\frac12\sigma^2x^2f_{xx}+\rho xf_x-\rho f=0.}
$$

Conversely, if the smooth function satisfies this equation, set $\delta=f_x$ and $\beta=(f-xf_x)/B$. Substituting into [Itô formula](../../../../../ito-s-lemma.md) gives exactly $df=\delta dS+\beta dB$, so these holdings are [self-financing](../../../../../self-financing-portfolio.md). This checks the holdings as well as the value equation; a [partial differential equation](../../../../../partial-differential-equation-split.md) solution does not justify arbitrary prescribed holdings. Appropriate admissibility and growth conditions are imposed when using it as an economic price.

For the [logarithmic stock payoff](../../../../../logarithmic-stock-payoff.md), let $\tau=T-t$ and condition on $S_t=x$. Under the [risk-neutral measure](../../../../../risk-neutral-measure.md),

$$
S_T=x e^{(\rho-\sigma^2/2)\tau+\sigma\sqrt\tau Z},\qquad Z\sim N(0,1).
$$

The normal exponential moment $\mathbb Ee^{uZ}=e^{u^2/2}$ and its derivative $\mathbb E[Ze^{uZ}]=u e^{u^2/2}$ give

$$
\mathbb E_Q[S_T\log S_T\mid S_t=x]
=xe^{\rho\tau}\bigl[\log x+(\rho+\sigma^2/2)\tau\bigr].
$$

Therefore

$$
\boxed{f(x,t)=x\bigl[\log x+(\rho+\sigma^2/2)(T-t)\bigr],\qquad
\delta_t=\log S_t+1+(\rho+\sigma^2/2)(T-t).}
$$

The [option delta](../../../../../option-delta.md) is the displayed [stock](../../../../../stock.md) holding. The [bank account](../../../../../bank-account.md) value is $f-S_tf_x=-S_t$, so $\beta_t=-S_t/B_t$. Directly, $f_{xx}=1/x$ and $f_t=-x(\rho+\sigma^2/2)$ verify the [partial differential equation](../../../../../partial-differential-equation-split.md), while $f(x,T)=x\log x$ verifies the payoff. Lognormal moments give the required pricing integrability. Since $x\log x\ge-1/e$, the conditional price is bounded below over this finite horizon, so the resulting [claim replication](../../../../../claim-replication.md) has the usual admissibility property.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
