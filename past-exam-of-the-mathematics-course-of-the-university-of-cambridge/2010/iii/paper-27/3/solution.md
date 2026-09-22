<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The common [Brownian motion](../../../../../brownian-motion-split.md) cancels from the difference $D_t=Y_t-X_t$. Before either lifetime,

$$
dD_t=a\left(\frac1{Y_t}-\frac1{X_t}\right)dt
=-\frac{aD_t}{X_tY_t}\,dt,
\qquad
D_t=(y-x)\exp\left(-a\int_0^t\frac{ds}{X_sY_s}\right)>0.
$$

Hence $0<X_t<Y_t$ and $\sigma\leq\tau$: if $Y$ reached zero first, the positive smaller solution $X$ could not persist beyond that time. Write

$$
\Theta_t=\frac{D_t}{Y_t}=1-\frac{X_t}{Y_t}\in(0,1),\qquad t<\sigma.
$$

Using the [Itô formula](../../../../../ito-s-lemma.md) for $Y^{-1}$ gives

$$
d(Y_t^{-1})=-Y_t^{-2}dB_t+(1-a)Y_t^{-3}dt.
$$

The difference has [finite variation](../../../../../total-variation-of-a-function.md), so there is no cross-variation term in the [Itô product rule](../../../../../ito-product-rule.md) for $D/Y$. Since $X=Y(1-\Theta)$,

$$
\boxed{d\Theta_t=-\frac{\Theta_t}{Y_t}dB_t
+\frac{\Theta_t}{Y_t^2}\left(1-a-\frac a{1-\Theta_t}\right)dt.}
$$

For $N_t=\chi(\Theta_t)$, the [Itô formula](../../../../../ito-s-lemma.md) therefore makes its drift vanish exactly when

$$
\frac12\theta^2\chi''(\theta)
+\theta\left(1-a-\frac a{1-\theta}\right)\chi'(\theta)=0.
$$

A nonconstant increasing [scale function of a one-dimensional diffusion](../../../../../scale-function-stochastic-processes.md) satisfies

$$
\frac{\chi''(\theta)}{\chi'(\theta)}
=-\frac{2-4a}{\theta}+\frac{2a}{1-\theta},
\qquad
\chi'(\theta)=C\theta^{4a-2}(1-\theta)^{-2a}.
$$

The assumptions $a>1/4$ and $a<1/2$ are precisely the integrability conditions at zero and one. Normalize the scale function by its endpoints:

$$
\boxed{\chi(\theta)=\phi(\theta)=
\frac{\displaystyle\int_0^\theta u^{4a-2}(1-u)^{-2a}\,du}
{\displaystyle\int_0^1 u^{4a-2}(1-u)^{-2a}\,du}
=I_\theta(4a-1,1-2a).}
$$

Here $I$ is the regularized [incomplete beta function](../../../../../incomplete-beta-function.md). The normalized function is continuous and strictly increasing on $[0,1]$, with $\phi(0)=0$ and $\phi(1)=1$. We have obtained the [local martingale](../../../../../local-martingale.md)

$$
\boxed{dN_t=-\frac{\Theta_t\phi'(\Theta_t)}{Y_t}\,dB_t,\qquad0\leq N_t\leq1.}
$$

The terminal identification needs care; mere boundedness does not by itself say what happens when both lifetimes coincide. Stop first on compact subsets of $0<X<Y$, and then exhaust the interval $[0,\sigma)$. The [bounded local martingale criterion](../../../../../bounded-local-martingale-criterion.md) makes $N$ a bounded [martingale](../../../../../martingale-split.md) with a limit $N_{\sigma-}$, and [optional sampling theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives $\mathbb E[N_{\sigma-}]=N_0$. For completeness, applying the [Itô formula](../../../../../ito-s-lemma.md) to each stopped $N^2$ bounds the expected [quadratic variation](../../../../../quadratic-variation.md) by one. [Monotone convergence](../../../../../monotone-convergence-theorem.md) over the localization sequence implies

$$
[N]_{\sigma-}=\int_0^\sigma\frac{\Theta_t^2\phi'(\Theta_t)^2}{Y_t^2}\,dt<\infty
\quad\text{almost surely}.
$$

Since $\phi^{-1}$ is continuous on $[0,1]$, $\Theta_t$ itself has a limit $\Theta_{\sigma-}$.

On $\{\sigma<\tau\}$, $Y_\sigma>0$ while $X_t\to0$, so $\Theta_{\sigma-}=1$ and $N_{\sigma-}=1$. On $\{\sigma=\tau\}$, the supplied divergent clock is

$$
\int_0^\sigma\frac{dt}{Y_t^2}=\infty.
$$

If $\Theta_{\sigma-}>0$, then eventually $\Theta_t\phi'(\Theta_t)$ is bounded below by a positive constant. This remains true if its limit is one: $\phi'(\theta)$ diverges there, rather than tending to zero. The divergent clock would then force $[N]_{\sigma-}=\infty$, contradicting the finite [quadratic variation](../../../../../quadratic-variation.md). Thus $\Theta_{\sigma-}=0$ and $N_{\sigma-}=0$ on the simultaneous-lifetime event. We have proved

$$
N_{\sigma-}=\mathbf1_{\{\sigma<\tau\}}.
$$

Taking expectations yields the complete [probability](../../../../../probability.md) formula

$$
\boxed{\mathbb P(\sigma<\tau)=\phi\!\left(\frac{y-x}{y}\right).}
$$

This is the [beta integral for strict ordering of coupled Bessel lifetimes](../../../../../beta-integral-for-strict-ordering-of-coupled-bessel-lifetimes.md); the complementary [probability](../../../../../probability.md) is the [probability](../../../../../probability.md) of simultaneous swallowing, not of the larger initial point dying first.

To connect the calculation to [SLE](../../../../../schramm-loewner-evolution.md), let its driver be $W_t=\sqrt\kappa\,\beta_t$. For a positive [boundary](../../../../../boundary-of-a-set.md) point $r$ before its [boundary swallowing time](../../../../../boundary-point-swallowing-time-for-a-loewner-chain.md), put $V_t^r=(g_t(r)-W_t)/\sqrt\kappa$. The [Chordal Loewner equation](../../../../../chordal-loewner-equation.md) gives

$$
dV_t^r=-d\beta_t+\frac{2/\kappa}{V_t^r}\,dt.
$$

Thus two positive [boundary](../../../../../boundary-of-a-set.md) points give exactly the coupled [Bessel processes](../../../../../bessel-process.md) above, with $B=-\beta$ and $a=2/\kappa$. The interval $1/4<a<1/2$ corresponds to $4<\kappa<8$. Their [boundary swallowing times](../../../../../boundary-point-swallowing-time-for-a-loewner-chain.md) obey

$$
\boxed{\mathbb P(T_x<T_y)=I_{1-x/y}\left(\frac8\kappa-1,1-\frac4\kappa\right),\qquad0<x<y.}
$$

The formula quantifies whether the growing hull separates one [boundary](../../../../../boundary-of-a-set.md) point from infinity before the other, or swallows them together inside the same [boundary](../../../../../boundary-of-a-set.md) interval. It does not identify swallowing with visiting each point. At $\kappa=6$, the two beta parameters are $1/3$ and this becomes the [Cardy boundary crossing formula](../../../../../cardy-boundary-crossing-formula.md) in the corresponding cross-ratio coordinate, explaining its role in the [conformal invariance of planar percolation](../../../../../conformal-invariance-of-planar-percolation.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
