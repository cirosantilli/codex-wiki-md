<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $A=\sigma\sigma^T$ and let $V(x,t)$ denote the optimal remaining expected reward from positive [portfolio wealth](../../../../../portfolio-wealth.md) $x$ at time $t$. The [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) and terminal condition are

$$
\boxed{V_t+\sup_{\theta\in\mathbb R^d,\ c\geq0}\left\{(\theta^T\mu-c)V_x+\frac12\theta^TA\theta\,V_{xx}+U_{\mathrm{consumption}}(c)\right\}=0,\qquad V(x,T)=U_{\mathrm{wealth}}(x).}
$$

The controls are progressively measurable, the investment integrals exist, consumption is nonnegative and locally integrable, and the resulting [portfolio wealth](../../../../../portfolio-wealth.md) stays in the utility domain. At zero consumption use the right limit of the [utility function](../../../../../utility-function-split.md) if needed. This is the usual [admissible trading strategy](../../../../../admissible-trading-strategy.md) formulation; without restrictions preserving the domain the reward need not be defined.

For the verification bound, assume $V$ is a nonnegative classical solution, continuous through the terminal time, with one time [derivative](../../../../../derivative.md) and two wealth [derivatives](../../../../../derivative.md) in the interior. Fix any admissible controls and put

$$
R_t=V(X_t,t)+\int_0^tU_{\mathrm{consumption}}(C_s)\,ds.
$$

The [Itô formula](../../../../../ito-s-lemma.md) gives

$$
dR_t=\left[V_t+(\theta_t^T\mu-C_t)V_x+\frac12\theta_t^TA\theta_tV_{xx}+U_{\mathrm{consumption}}(C_t)\right]dt+V_x\theta_t^T\sigma\,dW_t.
$$

The drift is nonpositive because the actual controls cannot exceed the supremum in the [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md). Localize by [stopping times](../../../../../stopping-time.md) on which the [stochastic integral](../../../../../stochastic-integral.md) is a true [martingale](../../../../../martingale-split.md), the derivatives and wealth stay in their interior domain, and the accumulated reward is finite. For each such stop $\tau_n$,

$$
\mathbb E R_{T\wedge\tau_n}\leq V(X_0,0).
$$

Both utilities and $V$ are nonnegative. Thus the [Fatou lemma](../../../../../fatou-s-lemma.md), continuity, and the terminal condition give

$$
\boxed{\mathbb E\left[U_{\mathrm{wealth}}(X_T)+\int_0^T U_{\mathrm{consumption}}(C_s)\,ds\right]\leq V(X_0,0).}
$$

For admissible paths strictly positive on the closed horizon, the domain-localizing stops eventually reach $T$. If zero wealth is allowed, the same proof uses the continuous boundary extension of $V$ and the utilities there. Nonnegativity is what permits removing the stops without assuming the uncontrolled stochastic term already has zero expectation. This is [verification by a nonnegative control supermartingale](../../../../../verification-by-a-nonnegative-control-supermartingale.md).

The square-root case needs an additional no-[arbitrage](../../../../../arbitrage.md) qualification because the printed volatility matrix need not be invertible. If there is $v\in\ker\sigma^T$ with $v^T\mu>0$, investment $\theta=Kv$ has zero volatility and arbitrarily large positive drift. With any fixed positive consumption, sufficiently large $K$ preserves positive wealth and makes terminal square-root utility tend to infinity. For example, in one dimension $\sigma=0$, $\mu=1$, $\theta=K$, $C=1$ gives $X_s=x+(K-1)(s-t)$, so the value is infinite when $T>t$. **A finite separated solution does not exist for all matrices allowed by the printed hypotheses.**

The needed condition is $\mu\in\operatorname{Range}A$, equivalent to $\mu$ being orthogonal to $\ker\sigma^T$, because $A$ is a [symmetric matrix](../../../../../symmetric-matrix.md) and $\ker A=\ker\sigma^T$. Assume this condition and let $B=A^+$ be its [Moore-Penrose inverse](../../../../../moore-penrose-inverse.md); if $A$ is invertible, simply use $B=A^{-1}$. Put $q=\mu^TB\mu\geq0$. Seek the [square-root investment-consumption value](../../../../../square-root-investment-consumption-value.md) in the form

$$
V(x,t)=2\sqrt{x}\,g(t),\qquad g(T)=1,\qquad g(t)>0.
$$

Then $V_x=g/\sqrt{x}$ and $V_{xx}=-g/(2x^{3/2})$. Completing the quadratic investment expression, using $AB\mu=\mu$, shows that its maximum is attained at $\theta^*=2xB\mu$ and has value $qg\sqrt{x}$:

$$
\frac{g}{\sqrt{x}}\theta^T\mu-\frac{g}{4x^{3/2}}\theta^TA\theta=qg\sqrt{x}-\frac{g}{4x^{3/2}}(\theta-2xB\mu)^TA(\theta-2xB\mu).
$$

Any investment component in $\ker A$ has no effect. For consumption, set $z=\sqrt c$. Its contribution is the concave quadratic $2z-(g/\sqrt{x})z^2$, whose maximum is $\sqrt{x}/g$ at $c^*=x/g^2$. Substituting both maxima into the [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) gives

$$
2g'+qg+\frac1g=0.
$$

With $h=g^2$, this becomes $h'+qh+1=0$, $h(T)=1$. Solving this linear [ordinary differential equation](../../../../../ordinary-differential-equation.md) gives

$$
\boxed{h(t)=\begin{cases}e^{q(T-t)}+\dfrac{e^{q(T-t)}-1}{q},&q>0,\\1+T-t,&q=0,\end{cases}\qquad V(x,t)=2\sqrt{x}\sqrt{h(t)}.}
$$

In particular $h\geq1$, so $g=\sqrt h$ stays positive, and the two controls are

$$
\boxed{\theta_t^*=2X_tB\mu,\qquad C_t^*=\frac{X_t}{h(t)}.}
$$

These controls are admissible and actually attain the value. Indeed their [portfolio wealth](../../../../../portfolio-wealth.md) satisfies

$$
\frac{dX_s}{X_s}=\left(2q-\frac1{h(s)}\right)ds+2\mu^TB\sigma\,dW_s.
$$

Since $\lVert2\mu^TB\sigma\rVert^2=4q$, the explicit positive solution starting at $(x,t)$ is

$$
X_s=x\exp\left[-\int_t^s\frac{dr}{h(r)}+2\mu^TB\sigma(W_s-W_t)\right].
$$

Its finite-horizon moments of every positive order are finite. More directly,

$$
\mathbb E\sqrt{X_s}=\sqrt{x}\exp\left[\frac q2(s-t)-\frac12\int_t^s\frac{dr}{h(r)}\right].
$$

Differentiating $g(s)\mathbb E\sqrt{X_s}$ and using the equation for $g$ gives $\frac{d}{ds}(g(s)\mathbb E\sqrt{X_s})=-\mathbb E\sqrt{X_s}/g(s)$. Integrating from $t$ to $T$ therefore yields

$$
\mathbb E\left[2\sqrt{X_T}+\int_t^T2\sqrt{C_s^*}\,ds\right]=2g(t)\sqrt{x}.
$$

This proves attainment without relying on an unjustified expectation of a local [martingale](../../../../../martingale-split.md). When $\mu$ is outside $\operatorname{Range}A$, the [singular-volatility drift arbitrage](../../../../../singular-volatility-drift-arbitrage.md) counterexample applies instead.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
