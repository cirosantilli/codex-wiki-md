<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the usual positive initial asset values. The coefficients determine a unique normalized [local martingale deflator](../../../../../../local-martingale-deflator.md). The [state-price density and local deflator distinction](../../../../../../state-price-density-and-local-deflator-distinction.md) matters here: calling it a [state-price density](../../../../../../state-price-density.md) uses the local convention, while true expectation pricing needs an additional qualification, addressed below.

Let $ZB$ and $ZS$ be [local martingales](../../../../../../local-martingale.md), with $Z_0=1$. The [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md) says that every [local martingale](../../../../../../local-martingale.md) in the usual [natural Brownian filtration](../../../../../../natural-brownian-filtration.md) is continuous and is a [stochastic integral](../../../../../../stochastic-integral.md) against $W$. Applying it to $ZB$, and dividing by the positive finite-variation account, forces

$$
dZ_t=-r_tZ_tdt+\eta_tdW_t
$$

for a locally square-integrable predictable $\eta$. The [Itô product rule](../../../../../../ito-product-rule.md) for $ZS$ has drift

$$
S_t\{Z_t(\mu_t-r_t)+\eta_t\sigma_t\}dt.
$$

It must vanish. Since $S,Z,\sigma$ are positive, this yields

$$
\boxed{\lambda_t=\frac{\mu_t-r_t}{\sigma_t},\qquad
\eta_t=-Z_t\lambda_t,\qquad dZ_t=-Z_t(r_tdt+\lambda_tdW_t).}
$$

Conversely this drift choice makes both $ZB$ and $ZS$ [local martingales](../../../../../../local-martingale.md). Continuity and strict positivity of $\sigma$ make $\lambda$ bounded along each path on every finite time interval, so its pathwise square integral is finite. The unique linear SDE solution is

$$
\boxed{Z_t=\exp\left(-\int_0^t r_sds-\int_0^t\lambda_sdW_s-\frac12\int_0^t\lambda_s^2ds\right)>0.}
$$

Uniqueness follows from the forced drift and diffusion coefficients and uniqueness of this linear [stochastic differential equation](../../../../../../stochastic-differential-equation.md).

**Continuity alone does not make the density a true [martingale](../../../../../../martingale-split.md).** For a true [equivalent martingale measure](../../../../../../risk-neutral-measure.md), the [stochastic exponential](../../../../../../doleans-dade-exponential.md) $D_t=Z_tB_t/B_0$ must have expectation one, for example under the [Novikov condition](../../../../../../novikov-s-condition.md) on each horizon. True [martingale](../../../../../../martingale-split.md) pricing of all desired deflated payoffs also requires the relevant integrability. These stronger conclusions do not follow just from pathwise continuity.

An explicit counterexample to the stronger reading uses a three-dimensional [Bessel process](../../../../../../bessel-process.md) $R$ with $R_0=1$ and $dR=dW+R^{-1}dt$, which is a positive strong solution in the Brownian filtration. Take $B=1$ and $S=R$. Then $r=0$, $\mu=R^{-2}$ and $\sigma=R^{-1}$ are continuous and $\sigma>0$. The unique local candidate is $Z=R^{-1}$, with $ZS=1$. The [reciprocal three-dimensional Bessel strict local martingale](../../../../../../reciprocal-three-dimensional-bessel-strict-local-martingale.md) is not a true [martingale](../../../../../../martingale-split.md). To verify the loss of expectation, use the standard Bessel transition density

$$
p_t(1,y)=\frac{y}{\sqrt{2\pi t}}\left(e^{-(y-1)^2/(2t)}-e^{-(y+1)^2/(2t)}\right),\qquad y>0.
$$

Integrating $p_t(1,y)/y$ gives $\mathbb E[R_t^{-1}]=2\Phi(1/\sqrt t)-1<1$ for $t>0$, where $\Phi$ is the [standard normal cumulative distribution function](../../../../../../standard-normal-distribution-function.md). A true pricing density for the constant bank account would have expectation one. Hence the printed hypotheses establish the local deflator statement, while a true-density reading needs an additional condition and is false as stated.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
