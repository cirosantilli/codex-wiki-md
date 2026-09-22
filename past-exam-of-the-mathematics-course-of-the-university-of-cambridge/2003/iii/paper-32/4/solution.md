<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume $\sigma>0$, $x>0$ and sufficient $C^{2,1}$ regularity to use the [Itô formula](../../../../../ito-s-lemma.md). Under the physical measure write $dS_t=\mu S_tdt+\sigma S_tdW_t$ and let the [bank account](../../../../../bank-account.md) be $R_t=e^{\rho t}$. If $V_t=f(S_t,t)$ is a [self-financing portfolio](../../../../../self-financing-portfolio.md) with $\Delta_t$ stock units and $\beta_t$ bank-account units, then

$$
dV_t=\Delta_t\,dS_t+\beta_t\,dR_t,\qquad V_t=\Delta_tS_t+\beta_tR_t.
$$

The [Itô formula](../../../../../ito-s-lemma.md) gives $df=(f_t+\mu S_tf_x+\tfrac12\sigma^2S_t^2f_{xx})dt+\sigma S_tf_xdW_t$. Equating diffusion terms forces $\Delta_t=f_x(S_t,t)$; equating drifts and eliminating $\beta_tR_t=f-S_tf_x$ gives the [Black-Scholes equation](../../../../../black-scholes-equation.md)

$$
\boxed{f_t+\tfrac12\sigma^2x^2f_{xx}+\rho x f_x-\rho f=0.}
$$

Conversely, if this equation holds, take $\Delta=f_x$ and $\beta=(f-xf_x)/R$. The same comparison shows $df=\Delta\,dS+\beta\,dR$, so the constructed portfolio is [self-financing](../../../../../self-financing-portfolio.md). This is a local replication equivalence for smooth functions on the state space; global admissibility and a terminal condition specify a unique economically admissible claim price.

With continuous stock-dividend yield $\theta$, holding $\Delta_t$ stock units earns $\theta\Delta_tS_tdt$ in addition to their price changes. A [self-financing portfolio](../../../../../self-financing-portfolio.md) reinvests that income, so

$$
dV_t=\Delta_t(dS_t+\theta S_tdt)+\beta_t\,dR_t.
$$

The same diffusion comparison gives $\Delta=f_x$, and the drift comparison yields the [Black-Scholes equation with continuous stock dividends](../../../../../black-scholes-equation-with-continuous-stock-dividends.md)

$$
\boxed{f_t+\tfrac12\sigma^2x^2f_{xx}+(\rho-\theta)xf_x-\rho f=0.}
$$

Under the [risk-neutral measure](../../../../../risk-neutral-measure.md), the ex-dividend stock consequently has drift $\rho-\theta$, while cash is discounted at $\rho$.

For the last claim, distinguish the terminal payoff function $F$ from a time-dependent price. Put $\tau=t_0-t$. The price with yield $\theta$ is $q(x,t)=e^{-\rho\tau}\mathbb E[F(xe^{(\rho-\theta-\sigma^2/2)\tau+\sigma\sqrt\tau Z})]$, with $Z$ a standard [normal random variable](../../../../../gaussian-random-variable.md). In a no-dividend model with interest rate $\rho-\theta$, the stock-transition law is identical but its discount factor is $e^{-(\rho-\theta)\tau}$. Thus, whenever the payoff expectation is finite, the [dividend-yield discount shift](../../../../../dividend-yield-discount-shift.md) gives

$$
\boxed{q(x,t)=e^{-\theta(t_0-t)}p(x,t).}
$$

Equivalently substitute this expression in the dividend equation: $q_t=e^{-\theta\tau}(p_t+\theta p)$, and the equation reduces exactly to the no-dividend [Black-Scholes equation](../../../../../black-scholes-equation.md) with rate $\rho-\theta$, with the same terminal data.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
