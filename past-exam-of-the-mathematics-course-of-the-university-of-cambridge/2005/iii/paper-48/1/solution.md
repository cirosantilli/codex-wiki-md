<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a discrete-time [martingale](../../../../../martingale-split.md) relative to the [filtration](../../../../../filtration-probability-theory.md) $(\mathcal F_n)$, each $M_n$ is $\mathcal F_n$-measurable, $\mathbb E|M_n|<\infty$, and $\mathbb E[M_n\mid\mathcal F_{n-1}]=M_{n-1}$ for $n\geq1$. The [tower property](../../../../../law-of-total-expectation.md) then gives the corresponding identity conditional on any earlier time.

A bounded [previsible process](../../../../../predictable-process.md) has $\phi_i$ measurable at time $i-1$ and $|\phi_i|\leq C$. Its [martingale transform](../../../../../martingale-transform.md) $V$ is adapted and integrable, since each increment has absolute expectation at most $C(\mathbb E|M_i|+\mathbb E|M_{i-1}|)$. Moreover,

$$
\mathbb E[V_n-V_{n-1}\mid\mathcal F_{n-1}]
=\phi_n\mathbb E[M_n-M_{n-1}\mid\mathcal F_{n-1}]=0.
$$

Thus **$V$ is a [martingale](../../../../../martingale-split.md)**, with $V_0=0$.

For the [Itô integral](../../../../../ito-integral.md), begin with a bounded adapted step integrand $H_s=H_i$ on $(t_i,t_{i+1}]$. Its integral is $I=\sum_iH_i(W_{t_{i+1}}-W_{t_i})$. Each summand has zero conditional [mean](../../../../../expected-value.md). For $i<j$, conditioning the cross product on $\mathcal F_{t_j}$ makes its expectation zero. The conditional second moment of a Brownian increment is $t_{i+1}-t_i$, hence

$$
\mathbb EI=0,\qquad \mathbb EI^2=\sum_i\mathbb E[H_i^2](t_{i+1}-t_i)
=\mathbb E\int_0^tH_s^2\,ds.
$$

Approximate the predictable integrand $g(s,W_s)$ in $L^2(ds\,d\mathbb P)$ by such step processes. The same identity makes their integrals Cauchy in $L^2$ and defines the limit; both its first and second moments converge. This gives the requested [mean](../../../../../expected-value.md)-zero result and the [Itô isometry](../../../../../ito-isometry.md):

$$
\boxed{\mathbb E\int_0^tg(s,W_s)dW_s=0,\qquad
\mathbb E\left(\int_0^tg(s,W_s)dW_s\right)^2=\mathbb E\int_0^tg(s,W_s)^2ds.}
$$

For the [Ornstein-Uhlenbeck process](../../../../../ornstein-uhlenbeck-process.md), the deterministic [integrating factor](../../../../../integrating-factor.md) has no [quadratic covariation](../../../../../quadratic-covariation.md) with $X$. The [Itô formula](../../../../../ito-s-lemma.md) therefore gives $d(e^{\kappa t}X_t)=\kappa\theta e^{\kappa t}dt+\sigma e^{\kappa t}dW_t$. Integrating and dividing by $e^{\kappa t}$ yields

$$
\boxed{X_t=\theta+(x-\theta)e^{-\kappa t}+\sigma\int_0^te^{-\kappa(t-s)}dW_s.}
$$

The [mean](../../../../../expected-value.md)-zero integral and [Itô isometry](../../../../../ito-isometry.md) give

$$
\boxed{\mathbb EX_t=\theta+(x-\theta)e^{-\kappa t},\qquad
\operatorname{Var}X_t=\frac{\sigma^2}{2\kappa}(1-e^{-2\kappa t}).}
$$

At $\kappa=0$ these formulas are read by continuity: $X_t=x+\sigma W_t$, with [mean](../../../../../expected-value.md) $x$ and [variance](../../../../../variance-split.md) $\sigma^2t$.

For the [CIR model](../../../../../cox-ingersoll-ross-model.md), let $C_0=c_0\geq0$ and use the usual positive parameters. Before a possible visit to zero, the derivatives of $\sqrt c$ are $1/(2\sqrt c)$ and $-1/(4c^{3/2})$. Applying the [Itô formula](../../../../../ito-s-lemma.md) gives the [Square root of a CIR diffusion](../../../../../square-root-of-a-cir-diffusion.md):

$$
\boxed{dZ_t=\left(\frac{4ab-\sigma^2}{8Z_t}-\frac a2Z_t\right)dt+\frac\sigma2dW_t.}
$$

The PDF's claim under $2ab=\sigma^2$ is false: that choice leaves the nonzero drift $\sigma^2/(8Z_t)-aZ_t/2$, which is not affine in $Z_t$. The actual interior cancellation condition is $4ab=\sigma^2$. Even then the principal square root is nonnegative and cannot be an unrestricted [Gaussian](../../../../../normal-distribution.md) [OU process](../../../../../ornstein-uhlenbeck-process.md).

To give the intended corrected construction, let a signed process solve $dY_t=-aY_tdt/2+(\sigma/2)dB_t$, with $Y_0=\sqrt{c_0}$. The [Itô formula](../../../../../ito-s-lemma.md) gives

$$
d(Y_t^2)=\left(\frac{\sigma^2}{4}-aY_t^2\right)dt+\sigma Y_t,dB_t.
$$

Writing $\widetilde W_t=\int_0^t\operatorname{sgn}(Y_s)dB_s$, with either sign chosen at zero, produces a [Brownian motion](../../../../../brownian-motion-split.md); the diffusion term is $\sigma|Y_t|d\widetilde W_t$. Thus $Y^2$ is a [CIR model](../../../../../cox-ingersoll-ross-model.md) with $ab=\sigma^2/4$, while $Z=|Y|$ is reflected at zero. The reflection contributes [local time of a semimartingale](../../../../../local-time-of-a-semimartingale.md), so the interior SDE alone is not a global unrestricted OU equation. Its second moment is $c_0e^{-at}+\sigma^2(1-e^{-at})/(4a)$, agreeing with the CIR [mean](../../../../../expected-value.md) for that corrected parameter choice.

The requested [mean](../../../../../expected-value.md) under the parameters actually printed is still available without the false OU assertion. Taking expectation in the original CIR equation gives $m'=a(b-m)$; the [stochastic integral](../../../../../stochastic-integral.md) has zero [mean](../../../../../expected-value.md) after the usual moment/localization justification. Consequently, for the printed choice as well as general admissible parameters,

$$
\boxed{\mathbb EC_t=b+(c_0-b)e^{-at}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
