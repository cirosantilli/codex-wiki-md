<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $M_t=\sup_{s\leq t}W_s$ and write $\phi_t(y)=(2\pi t)^{-1/2}e^{-y^2/(2t)}$ for the Brownian terminal density. By the [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md), for $y<a$ the reflected paths that hit $a$ and end at $y$ have terminal density $\phi_t(2a-y)$. Hence

$$
P(M_t\leq a,\ W_t\in dy)=[\phi_t(y)-\phi_t(2a-y)]\mathbf1_{\{y<a\}}dy.
$$

The [Girsanov theorem](../../../../../girsanov-theorem.md) changes zero drift into drift $\nu$ using the finite-horizon density $e^{\nu W_t-\nu^2t/2}$. The [finite-horizon maximum of Brownian motion with drift](../../../../../finite-horizon-maximum-of-brownian-motion-with-drift.md) therefore has distribution function

$$
\begin{aligned}
P\left(\sup_{s\leq t}(W_s+\nu s)\leq a\right)
&=\int_{-\infty}^a e^{\nu y-\nu^2t/2}[\phi_t(y)-\phi_t(2a-y)]\,dy\\
&=\boxed{\Phi\left(\frac{a-\nu t}{\sqrt t}\right)-e^{2a\nu}\Phi\left(\frac{-a-\nu t}{\sqrt t}\right)}.
\end{aligned}
$$

In the first integral term, complete the square to get a normal density with mean $\nu t$. In the second, substitute $z=2a-y$ and complete the square with mean $-\nu t$; the prefactor is $e^{2a\nu}$. Here $\Phi$ is the [standard normal distribution function](../../../../../standard-normal-distribution-function.md), $a>0$ and $t>0$.

Let $T_{a,b}=\inf\{s\geq0:W_s=a+bs\}$, with $b$ real. Survival means that $W_s-bs$ stays below $a$. Tilt by $e^{\theta W_t-\theta^2t/2}$; under the tilted probability, $W_s$ has drift $\theta$. Applying the maximum formula with drift $\theta-b$ gives the [exponential terminal moment below a linear Brownian boundary](../../../../../exponential-terminal-moment-below-a-linear-brownian-boundary.md)

$$
\boxed{\mathbb E[e^{\theta W_t}\mathbf1_{\{T_{a,b}>t\}}]=e^{\theta^2t/2}\left[\Phi\left(\frac{a+(b-\theta)t}{\sqrt t}\right)-e^{2a(\theta-b)}\Phi\left(\frac{-a+(b-\theta)t}{\sqrt t}\right)\right].}
$$

This holds for every real $\theta$. The maximum distribution has no atom at the positive barrier, so strict or weak survival inequalities give the same probability here.

For the hitting-time moment, first use drift $-b$ in the maximum formula and take the complementary probability:

$$
F_b(t)=P(T_{a,b}\leq t)=\Phi\left(\frac{-a-bt}{\sqrt t}\right)+e^{-2ab}\Phi\left(\frac{-a+bt}{\sqrt t}\right).
$$

If $z_1=(-a-bt)/\sqrt t$ and $z_2=(-a+bt)/\sqrt t$, their standard normal densities satisfy $\phi(z_1)=e^{-2ab}\phi(z_2)$. Differentiating the two terms, with $z_1'=(a-bt)/(2t^{3/2})$ and $z_2'=(a+bt)/(2t^{3/2})$, yields the [drifted Brownian first-passage density](../../../../../drifted-brownian-first-passage-density.md)

$$
f_b(s)=\frac{a}{\sqrt{2\pi s^3}}\exp\left[-\frac{(a+bs)^2}{2s}\right],\qquad s>0.
$$

Its total mass need not be one, because the upward-sloping boundary may never be reached.

For $2\theta\leq b^2$, put $\kappa=\sqrt{b^2-2\theta}\geq0$. Multiplication by $e^{\theta s}$ gives $e^{\theta s}f_b(s)=e^{a(\kappa-b)}f_\kappa(s)$. Integrating to $t$ produces [truncated discounted Brownian first passage](../../../../../truncated-discounted-brownian-first-passage.md), with negative discount rate allowed when the square root remains real:

$$
\boxed{\mathbb E[e^{\theta T_{a,b}}\mathbf1_{\{T_{a,b}\leq t\}}]=e^{a(\kappa-b)}\Phi\left(\frac{-a-\kappa t}{\sqrt t}\right)+e^{-a(\kappa+b)}\Phi\left(\frac{-a+\kappa t}{\sqrt t}\right).}
$$

This includes the equality case $\kappa=0$, where it becomes $2e^{-ab}\Phi(-a/\sqrt t)$. The expression integrates only finite hitting times up to $t$; no value is assigned to an exponential at an infinite hitting time.

For the [cash-at-hit digital call](../../../../../cash-at-hit-digital-call.md), use the [risk-neutral measure](../../../../../risk-neutral-measure.md) in the [Black-Scholes model](../../../../../black-scholes-model.md) and denote expiry by $T=t_0$. Then

$$
\log(S_s/S_0)=(\rho-\sigma^2/2)s+\sigma W_s^Q.
$$

Hitting $c>S_0$ corresponds to $W_s^Q=a+bs$, where $a=\log(c/S_0)/\sigma>0$ and $b=(\sigma^2/2-\rho)/\sigma$. The unit-cash payment is made at the hitting time, so [risk-neutral valuation](../../../../../risk-neutral-pricing.md) discounts at that time, not at expiry. Set $\theta=-\rho$ and

$$
\kappa=\sqrt{b^2+2\rho}=\frac{|\rho+\sigma^2/2|}{\sigma}.
$$

The identity on the right verifies the square-root condition even for negative interest rates. The time-zero price is

$$
\boxed{D_0=e^{a(\kappa-b)}\Phi\left(\frac{-a-\kappa T}{\sqrt T}\right)+e^{-a(\kappa+b)}\Phi\left(\frac{-a+\kappa T}{\sqrt T}\right).}
$$

This is in pounds for the unit-pound contract. It differs from a maturity-paid [digital call option](../../../../../digital-call-option.md), whose discounting and exercise event are different.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
