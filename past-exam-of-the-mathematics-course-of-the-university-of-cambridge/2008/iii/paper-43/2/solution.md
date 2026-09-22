<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Under [quota share reinsurance](../../../../../quota-share-reinsurance.md), the direct insurer retains a fixed fraction $\alpha$ of each claim and the reinsurer pays the other fraction. Thus their annual claim totals are $\alpha S$ and $(1-\alpha)S$. Under [excess of loss reinsurance](../../../../../excess-of-loss-reinsurance.md) with retention $d$, the direct insurer pays $\min(X_j,d)$ on each individual claim and the reinsurer pays $(X_j-d)_+$. Under [stop loss reinsurance](../../../../../aggregate-stop-loss-reinsurance.md) with annual retention $D$, the direct insurer pays $\min(S,D)$ and the reinsurer pays $(S-D)_+$. The last two contracts differ because one caps each claim and the other caps the aggregate.

Conditioning on the annual [Poisson distribution](../../../../../poisson-distribution.md) count gives the [compound Poisson distribution](../../../../../compound-poisson-distribution.md) transform:

$$
M_S(t)=\sum_{n\ge0}e^{-\lambda}\frac{\lambda^n}{n!}M_X(t)^n
=\boxed{\exp\{\lambda(M_X(t)-1)\}.}
$$

This equality is understood on the domain where the [moment-generating function](../../../../../moment-generating-function.md) is finite. By the [expected value premium principle](../../../../../expected-value-premium-principle.md), annual premium income is $c=(1+\theta)\lambda\mu$. Without [reinsurance](../../../../../reinsurance.md), final capital is $W_0=u+c-S$, and therefore

$$
\boxed{M_{W_0}(t)=\exp\{t(u+(1+\theta)\lambda\mu)+\lambda(M_X(-t)-1)\}.}
$$

For the quota-share contract, the reinsurer's expected claim cost is $(1-\alpha)\lambda\mu$, so its annual premium is

$$
\boxed{c_R=(1+\theta_R)(1-\alpha)\lambda\mu.}
$$

The direct insurer keeps its original premium income, pays this reinsurance premium and retains only $\alpha S$. Thus

$$
W=u+c-c_R-\alpha S
=u+\lambda\mu\{\theta-\theta_R+(1+\theta_R)\alpha\}-\alpha S,
$$

and

$$
\boxed{M_W(t)=\exp\left[t\left(u+\lambda\mu\{\theta-\theta_R+(1+\theta_R)\alpha\}\right)
+\lambda\{M_X(-\alpha t)-1\}\right].}
$$

The reinsurer's loading is applied to the ceded expected loss, not to the direct insurer's original premium.

Maximizing expected [exponential utility](../../../../../constant-absolute-risk-aversion-utility.md) $\mathbb E[-e^{-\beta W}]$ is equivalent to minimizing the exponent $H(\alpha)=\log\mathbb E[e^{-\beta W}]$. For [exponential distribution](../../../../../exponential-distribution.md) claim sizes of mean $\mu$,

$$
M_X(r)=\frac1{1-\mu r},\qquad r<1/\mu,
$$

so on the finite-utility domain $\beta\mu\alpha<1$,

$$
H(\alpha)=-\beta\left[u+\lambda\mu\{\theta-\theta_R+(1+\theta_R)\alpha\}\right]
+\lambda\left(\frac1{1-\beta\mu\alpha}-1\right).
$$

For a nontrivial positive arrival rate, differentiation gives

$$
H'(\alpha)=\lambda\beta\mu\left[(1-\beta\mu\alpha)^{-2}-(1+\theta_R)\right],
\qquad
H''(\alpha)=\frac{2\lambda(\beta\mu)^2}{(1-\beta\mu\alpha)^3}>0.
$$

The unique unconstrained stationary retention is therefore

$$
\boxed{\alpha_*=
\frac{1-(1+\theta_R)^{-1/2}}{\beta\mu}.}
$$

It is positive and lies below $1/(\beta\mu)$. If $\alpha_*<1$, it is the unique optimal retention in the printed range $0<\alpha<1$. If $\alpha_*\ge1$, expected utility increases throughout that open interval and its supremum is approached as $\alpha\uparrow1$; **there is no attained maximum in the strictly open range**. Allowing the usual no-reinsurance endpoint gives the compact formula

$$
\boxed{\alpha_{\mathrm{opt}}=\min\{1,\alpha_*\}\quad\text{when }0\le\alpha\le1.}
$$

Retentions with $\beta\mu\alpha\ge1$ have infinite exponential loss moment and expected utility $-\infty$, so they cannot displace the finite stationary solution. The stationary point and full-retention endpoint just described stay within the finite-transform domain whenever they are selected.

For the requested comparisons,

$$
\frac{\partial\alpha_*}{\partial\theta_R}
=\frac{1}{2\beta\mu(1+\theta_R)^{3/2}}>0.
$$

**Higher reinsurer loading increases optimal retention**, up to full retention: reinsurance is more expensive. **The direct insurer's loading $\theta$ does not affect the optimizer**. It adds only the constant $-\beta\lambda\mu\theta$ to $H$, reflecting the translation property of constant absolute risk aversion. These observations give the [quota-share retention under exponential utility](../../../../../quota-share-retention-under-exponential-utility.md) rule; $u$ and the positive arrival rate also drop out of the stationary equation. In the degenerate case $\lambda=0$, no claims or premiums occur, $W=u$, and every retained fraction has the same expected utility.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
