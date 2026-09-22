<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use $U_t=2W_t$ and write $Z_t=X_t+iY_t$ up to its [interior-point swallowing time for a Loewner chain](../../../../../interior-point-swallowing-time-for-a-loewner-chain.md) $T_z$. The [Chordal Loewner equation](../../../../../chordal-loewner-equation.md) gives

$$
dZ_t=\frac2{Z_t}\,dt-2\,dW_t,\qquad
 dY_t=-\frac{2Y_t}{|Z_t|^2}\,dt.
$$

The branch of the [complex logarithm](../../../../../complex-logarithm.md) with argument in $(0,\pi)$ is well-defined while $t<T_z$. The [Itô formula](../../../../../ito-s-lemma.md) yields the crucial cancellation

$$
\boxed{d\log Z_t=\frac1{Z_t}dZ_t-\frac1{2Z_t^2}d[Z]_t
=-\frac2{Z_t}\,dW_t.}
$$

The $2/Z_t^2$ drift is cancelled by the [quadratic variation](../../../../../quadratic-variation.md) term, because $\kappa=4$. Thus both $L_t=\log|Z_t|$ and $\theta_t=\arg Z_t$ are continuous [local martingales](../../../../../local-martingale.md), with

$$
dL_t=-\frac{2X_t}{|Z_t|^2}\,dW_t,\qquad
 d\theta_t=\frac{2Y_t}{|Z_t|^2}\,dW_t.
$$

This is the [logarithmic martingale for SLE4](../../../../../logarithmic-martingale-for-sle4.md).

We justify absence of a finite swallowing time rather than presuming that the logarithm survives forever. On a finite horizon $H$, $0<Y_t\leq\operatorname{Im}z$. Also $|X_t|$ is bounded pathwise before $T_z\wedge H$. Indeed, while $|X_t|\geq1$ its drift $2X_t/|Z_t|^2$ has absolute value at most $2$; on each excursion outside $[-1,1]$, integrate from its starting point and bound the Brownian oscillation on $[0,H]$. For example,

$$
|X_t|\leq\max(1,|\operatorname{Re}z|)+2H+4\sup_{s\leq H}|W_s|.
$$

Therefore $L_t$ is bounded above pathwise on this interval.

Suppose $T_z\leq H$. By the [Dambis-Dubins-Schwarz theorem](../../../../../dambis-dubins-schwarz-theorem.md), $L$ is a [Brownian motion](../../../../../brownian-motion-split.md) run at its own [quadratic variation](../../../../../quadratic-variation.md). If that clock diverged as $t\uparrow T_z$, Brownian oscillation would make $L$ unbounded above, contradicting the preceding bound. The [one-sided bound criterion for a martingale clock](../../../../../one-sided-bound-criterion-for-a-martingale-clock.md) therefore gives a finite clock limit and a finite real limit for $L_t$. Hence $|Z_t|$ is bounded away from zero near $T_z$.

Now $Y_t=Y_0\exp(-2\int_0^t|Z_s|^{-2}ds)$ has a strictly positive limit at $T_z$. The drift in $X$ is integrable there, so continuity of $W$ gives a finite limit for $X$ as well. The limiting point is in $\mathbb H$ and away from the [Loewner driver](../../../../../loewner-driving-function.md) singularity, and the differential equation extends past $T_z$, a contradiction. Thus **$T_z=\infty$ almost surely**. A point of the [Loewner trace](../../../../../trace-of-a-loewner-chain.md) at a finite time belongs to that time's hull, so

$$
\boxed{\mathbb P\{z\in\gamma^*\}=0.}
$$

This proves the [fixed-interior-point avoidance of SLE4](../../../../../fixed-interior-point-avoidance-of-sle4.md) without using simplicity as an input.

The angle remains in $(0,\pi)$ at all finite times. The [bounded local martingale criterion](../../../../../bounded-local-martingale-criterion.md) upgrades its [local martingale](../../../../../local-martingale.md) equation to a genuine [martingale](../../../../../martingale-split.md):

$$
\boxed{\mathbb E[\theta_t\mid\mathcal F_s]=\theta_s,\qquad
\mathbb E\theta_t=\arg z.}
$$

In particular this is the [SLE4 angle martingale](../../../../../sle4-angle-martingale.md), and it converges almost surely and in $L^1$ by bounded [martingale convergence theorem](../../../../../martingale-convergence-theorem.md).

It remains to identify the limiting angle using the assumed simple path tending to infinity. Orient that path from $0$ to infinity. Its left component is the one adjacent to the negative real half-axis. Under $g_t$, the left boundary of the slit domain maps to $(-\infty,U_t)$ and the right boundary to $(U_t,\infty)$. The [harmonic measure](../../../../../harmonic-measure.md) of the former as seen from $z$ is

$$
\frac{\arg(g_t(z)-U_t)}\pi=\frac{\theta_t}{\pi}.
$$

This follows by [conformal invariance of planar Brownian motion](../../../../../conformal-invariance-of-planar-brownian-motion.md): in the upper half-plane, $\arg(w-U_t)/\pi$ is the bounded [harmonic function](../../../../../harmonic-function.md) with values $1$ on the left half-axis and $0$ on the right.

To justify the limiting boundary classification, condition on a simple proper realization of the path and use an independent [planar Brownian motion](../../../../../planar-brownian-motion.md) from $z$. It exits the upper half-plane in finite time almost surely, so its path up to that time is compact. The curve tends to infinity, so its intersection with this compact set is contained in a finite initial curve segment. Once that segment has been drawn, the Brownian path exits the slit domain through its left boundary exactly when $z$ is in the final left component: a path from that component cannot reach the right boundary without crossing the curve, and the reverse assertion holds on the right. Endpoints have zero harmonic measure. Bounded convergence of these exit indicators proves

$$
\theta_t\longrightarrow\pi\,1_{\{z\text{ is in the left component}\}}.
$$

Taking expectations in the bounded angle [martingale](../../../../../martingale-split.md) gives the [SLE4 left-passage probability](../../../../../sle4-left-passage-probability.md)

$$
\boxed{\mathbb P\{z\text{ is in the left component}\}
=\frac{\arg z}{\pi}
=\frac12-\frac1\pi\arctan\!\left(\frac{\operatorname{Re}z}{\operatorname{Im}z}\right).}
$$

For the imaginary axis it is $1/2$; near the negative real axis it tends to $1$, fixing the orientation of “left”.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
