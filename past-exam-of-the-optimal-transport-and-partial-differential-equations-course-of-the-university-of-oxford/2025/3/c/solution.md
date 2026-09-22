<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**A finite first moment suffices for the velocity, but may not suffice for the printed potential.** For example, $W(z)=|z|^2/2$ has all the stated properties. If $\mu$ is the law of $(S,0)$ with density $2s^{-3}$ on $s\geq1$, then $\mathbb ES=2$ but $\mathbb ES^2=\infty$, and $(W*\mu)(x)=\infty$ for every $x$. Thus the literal definition of $V$ needs a finite second [absolute moment](../../../../absolute-moment.md), or another hypothesis ensuring integrability of $W$.

For the specified class $\mathcal P_1$, define the [velocity fields](../../../../velocity-field.md) directly by $b_\mu=K*\mu$ and $b_{\widehat\mu}=K*\widehat\mu$. Equivalently, use the [renormalized interaction potential](../../../../renormalized-interaction-potential.md)

$$
V_{\mathrm{ren}}(t,x)=\int\left[W(x-z)-W(-z)\right]d\mu_t(z).
$$

The bounded [Hessian matrix](../../../../hessian-matrix.md) and $\nabla W(0)=0$ imply

$$
|W(x-z)-W(-z)|\leq L|x||z|+\frac L2|x|^2.
$$

Thus $V_{\mathrm{ren}}$ is finite, is twice continuously differentiable in space, and has $\nabla V_{\mathrm{ren}}=\nabla W*\mu$, by dominated [differentiation under the integral sign](../../../../differentiation-under-the-integral-sign.md). Its rotated negative [gradient](../../../../gradient.md) is exactly $b_\mu$. Whenever $W*\mu$ is finite, the two potentials differ only by an $x$-independent constant and give the same [transport equation](../../../../transport-equation-split.md).

We check the hypotheses for [characteristic representation of a measure-valued continuity equation](../../../../characteristic-representation-of-a-measure-valued-continuity-equation.md). For every $x,y$,

$$
|b_\mu(t,x)-b_\mu(t,y)|\leq L|x-y|,\qquad |b_\mu(t,x)|\leq L\left(|x|+m_1(\mu_t)\right),\qquad m_1(\mu_t)=\int|z|\,d\mu_t(z).
$$

For any [coupling](../../../../coupling.md) $\gamma\in\Gamma(\mu_t,\widehat\mu_t)$, the [Lipschitz condition](../../../../lipschitz-continuity.md) on $K$ also gives

$$
\begin{aligned}
|b_\mu(t,x)-b_{\widehat\mu}(t,x)|&=\left|\int[K(x-z)-K(x-\widehat z)]\,d\gamma(z,\widehat z)\right|\\
&\leq L\int|z-\widehat z|\,d\gamma(z,\widehat z).
\end{aligned}
$$

Taking the infimum over [couplings](../../../../coupling.md) proves the uniform bound

$$
\boxed{\sup_x|b_\mu(t,x)-b_{\widehat\mu}(t,x)|\leq Ld_1(\mu_t,\widehat\mu_t).}
$$

Applying the same estimate at two times of one curve proves time continuity of $b_\mu$, uniformly in $x$. Also $|m_1(\mu_t)-m_1(\mu_s)|\leq d_1(\mu_t,\mu_s)$, so $m_1(\mu_t)$ is bounded on compact time intervals. Spatial [partial derivatives](../../../../partial-derivative.md) of $b_\mu$ are continuous and bounded by $L$, using dominated convergence in space and [weak convergence of probability measures](../../../../weak-convergence-of-probability-measures.md) in time for the bounded continuous kernel $DK$. All corresponding facts hold for $\widehat\mu$.

The [characteristic representation of a measure-valued continuity equation](../../../../characteristic-representation-of-a-measure-valued-continuity-equation.md) says that a continuous [velocity field](../../../../velocity-field.md), continuously differentiable and globally [Lipschitz](../../../../lipschitz-continuity.md) in space and with locally uniform linear growth, has a global [characteristic flow map](../../../../characteristic-flow-map.md) $X_\mu(t;s,a)$ solving

$$
\frac d{dt}X_\mu(t;s,a)=b_\mu(t,X_\mu(t;s,a)),\qquad X_\mu(s;s,a)=a.
$$

For each $f\in\mathcal P_1$, its [pushforward measure](../../../../pushforward-measure.md) is the unique [weak solution](../../../../weak-solution.md) in $C([0,\infty),\mathcal P_1)$ of the associated [continuity equation](../../../../continuity-equation.md). The hypotheses have all been verified above, and the fields have zero [divergence](../../../../divergence.md), so these are also the two required [transport equations](../../../../transport-equation-split.md). Explicitly,

$$
\boxed{\rho_t=X_\mu(t;0,\cdot)_\#f,\qquad\widehat\rho_t=X_{\widehat\mu}(t;0,\cdot)_\#f.}
$$

For completeness, the [Gronwall inequality](../../../../gronwall-inequality.md) gives

$$
|X_\mu(t;0,a)|\leq e^{Lt}|a|+L\int_0^te^{L(t-s)}m_1(\mu_s)\,ds,
$$

so these [pushforward measures](../../../../pushforward-measure.md) have finite first [absolute moments](../../../../absolute-moment.md). Integrating $|X_\mu(t;0,a)-X_\mu(s;0,a)|$ against $f$ proves continuity in the [Wasserstein distance](../../../../wasserstein-distance.md). The [chain rule](../../../../chain-rule.md) proves the weak identity. For uniqueness at a fixed terminal time $t$, use the backward [test function](../../../../test-function.md) $\varphi(s,x)=\psi(X_\mu(t;s,x))$, where $\psi$ is continuously differentiable with compact [support](../../../../support.md). It satisfies $\partial_s\varphi+b_\mu\cdot\nabla\varphi=0$ and has compact spatial [support](../../../../support.md) uniformly for $0\leq s\leq t$, by the backward linear-growth bound. The weak identity with temporal cutoffs therefore gives $\int\psi\,d\rho_t=\int\psi(X_\mu(t;0,a))\,df(a)$, identifying every [weak solution](../../../../weak-solution.md) with the displayed [pushforward measure](../../../../pushforward-measure.md).

Finally compare the two [characteristic curves](../../../../characteristic-curve.md) with the same initial point $a$. Put $\Delta_t=X_\mu(t;0,a)-X_{\widehat\mu}(t;0,a)$. The spatial [Lipschitz condition](../../../../lipschitz-continuity.md) and the boxed velocity estimate give

$$
\frac d{dt}|\Delta_t|\leq L|\Delta_t|+Ld_1(\mu_t,\widehat\mu_t),\qquad\Delta_0=0,
$$

for almost every time; the integral form gives the same conclusion at zeros of $\Delta$. The [Gronwall inequality](../../../../gronwall-inequality.md) implies

$$
|\Delta_t|\leq L\int_0^te^{L(t-s)}d_1(\mu_s,\widehat\mu_s)\,ds.
$$

The [pushforward measure](../../../../pushforward-measure.md) $(X_\mu(t;0,\cdot),X_{\widehat\mu}(t;0,\cdot))_\#f$ is a [coupling](../../../../coupling.md) of $\rho_t,\widehat\rho_t$. Integrating the last bound against the [probability measure](../../../../probability-measure.md) $f$ proves

$$
\boxed{d_1(\rho_t,\widehat\rho_t)\leq L\int_0^te^{L(t-s)}d_1(\mu_s,\widehat\mu_s)\,ds.}
$$

The same constant $L$ depends only on the uniform bound for the [Hessian matrix](../../../../hessian-matrix.md) of $W$, and is independent of the prescribed curves and their common initial data.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the optimal transport and partial differential equations course of the University of Oxford](../../../split.md)
5. [Optimal transport and partial differential equations course of the University of Oxford](../../../../optimal-transport-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
