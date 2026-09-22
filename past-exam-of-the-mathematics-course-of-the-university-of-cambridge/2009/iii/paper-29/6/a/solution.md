<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [diffusion generator](../../../../../../diffusion-generator.md) is $\mathcal Lf=\tfrac12\sigma^2f''+bf'$. On a compact subinterval of $I$, the coefficient $s'\sigma$ is bounded, and the [Itô formula](../../../../../../ito-s-lemma.md) up to its exit time $\rho$ gives

$$
\boxed{s(X_{t\wedge\rho})=s(X_0)+\int_0^{t\wedge\rho}s'(X_u)\sigma(X_u)dB_u,}
$$

because $\mathcal Ls=0$. Increasing compact subintervals proves the local-martingale property up to $T$. The notation $s(X_{t\wedge T})$ at an exit endpoint is understood with its continuous endpoint extension when needed; stopping on $[a,b]\subset I$ below is always well-defined. This is the [martingale](../../../../../../martingale-split.md) property of a [scale function of a one-dimensional diffusion](../../../../../../scale-function-stochastic-processes.md).

For the hitting ratio there are two necessary qualifications: $s(b)\ne s(a)$ and $\tau=T_a\wedge T_b<\infty$ almost surely. A usual scale function is strictly monotone, which ensures the first condition, but the printed hypotheses alone ensure neither. Under these conditions, $s(X_{t\wedge\tau})$ is a bounded [local martingale](../../../../../../local-martingale.md) and hence a [uniformly integrable](../../../../../../uniform-integrability.md) [martingale](../../../../../../martingale-split.md). The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
s(x)=\mathbb Es(X_\tau)=s(a)\mathbb P(T_a<T_b)+s(b)\mathbb P(T_b<T_a).
$$

Continuity prevents simultaneous hitting of distinct endpoints, and almost sure exit makes these two probabilities sum to one. Solving yields the [boundary hitting probability from a diffusion scale function](../../../../../../boundary-hitting-probability-from-a-diffusion-scale-function.md)

$$
\boxed{\mathbb P(T_b<T_a)=\frac{s(x)-s(a)}{s(b)-s(a)}\quad\text{when exit is a.s. finite and }s(b)\ne s(a).}
$$

The [hypotheses for a diffusion scale hitting formula](../../../../../../hypotheses-for-a-diffusion-scale-hitting-formula.md) cannot be omitted here. Take $\sigma\equiv0$, drift $b\equiv0$, $s(y)=y$ and $X_t\equiv x\in(a,b)$. All printed coefficient and differential conditions hold, but neither endpoint is ever reached, so the left side is zero whereas the displayed ratio is strictly positive. A constant $s$ is another allowed solution of the printed differential equation and makes its denominator zero. In general the bounded stopped [martingale](../../../../../../martingale-split.md) has a limit $Y_\infty$, and optional stopping instead gives

$$
s(x)=s(a)\mathbb P(T_a<T_b)+s(b)\mathbb P(T_b<T_a)+\mathbb E[Y_\infty\mathbf1_{\{\tau=\infty\}}].
$$

The following parts have nondegenerate diffusion and strictly monotone powers, and their finite-exit properties are justified explicitly.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
