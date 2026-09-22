<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $g_t=g_{K_t}$ and, for $s<t$, let $K_{s,t}$ be the filled image hull $g_s(K_t\setminus K_s)$. The [half-plane-capacity composition rule](../../../../../half-plane-capacity-composition-rule.md) gives

$$
g_t=g_{K_{s,t}}\circ g_s,\qquad\operatorname{hcap}(K_{s,t})=2(t-s).
$$

The [Loewner local growth property](../../../../../loewner-local-growth-property.md) says that these mapped increments shrink uniformly on bounded time intervals: for every $A<\infty$,

$$
\omega_A(h):=\sup_{0\leq s<t\leq A,\ t-s\leq h}\operatorname{rad}(K_{s,t})\longrightarrow0
\quad\text{as }h\downarrow0.
$$

Using [diameter](../../../../../diameter.md) instead of radius is equivalent, since a nonempty [compact H-hull](../../../../../compact-h-hull.md) has its closure meeting the real axis. This is a condition on the increments after mapping out the past, not merely on the Euclidean size of $K_t\setminus K_s$ in the original domain.

For fixed $t$, the nonempty compact sets $\overline{K_{t,t+h}}$, $h>0$, are nested as $h$ decreases. Their diameters tend to zero by [Loewner local growth property](../../../../../loewner-local-growth-property.md). The nested-compact-set property gives a single intersection point, and its imaginary part is zero because $K_{t,t+h}$ lies in a real-centred disc of radius tending to zero. Define the [Loewner transform](../../../../../loewner-driving-function.md) by

$$
\boxed{\{\xi_t\}=\bigcap_{h>0}\overline{K_{t,t+h}},\qquad\xi_t\in\mathbb R.}
$$

One may restrict the intersection to sufficiently small $h$. Every point of $K_{t,t+h}$ is within $2\omega_A(h)$ of $\xi_t$ when $t+h\leq A$.

Here is a direct proof of [continuity](../../../../../continuous-function.md), using the permitted displacement estimate. Fix $s<t$ and put $\delta=t-s$. Take $0<h\leq\delta$ and a point $v\in K_{t,t+h}$. Set $z=g_{K_{s,t}}^{-1}(v)$. The hull composition rule puts $z\in K_{s,t+h}$, while the displacement estimate gives

$$
|v-z|\leq C\operatorname{rad}(K_{s,t})\leq C\omega_A(\delta).
$$

Since $z$ is within $2\omega_A(\delta+h)$ of $\xi_s$, let $h\downarrow0$, taking $v\to\xi_t$, to obtain

$$
\boxed{|\xi_t-\xi_s|\leq C\omega_A(\delta)+2\omega_A(2\delta).}
$$

Use a slightly larger fixed time interval if $t$ is its endpoint. Both terms tend to zero with $\delta$. This proves [continuity](../../../../../continuous-function.md) from both sides, and indeed [uniform continuity](../../../../../uniform-continuity.md) on every compact time interval. The real [boundary](../../../../../boundary-of-a-set.md) value is obtained as a limit; evaluating the displacement estimate directly on a possibly rough [boundary](../../../../../boundary-of-a-set.md) is unnecessary.

The [Loewner correspondence theorem](../../../../../loewner-correspondence-theorem.md) states that a capacity-$2t$ increasing hull family with [Loewner local growth property](../../../../../loewner-local-growth-property.md) has the unique continuous real [Loewner driving function](../../../../../loewner-driving-function.md) just defined, and its [mapping-out functions](../../../../../mapping-out-function-of-a-compact-h-hull.md) solve the [Chordal Loewner equation](../../../../../chordal-loewner-equation.md)

$$
\boxed{\partial_tg_t(z)=\frac2{g_t(z)-\xi_t},\qquad g_0(z)=z.}
$$

For each $z\in\mathbb H$, this solution is taken up to its maximal lifetime; $\mathbb H\setminus K_t$ is precisely the set of points whose lifetimes exceed $t$. Conversely a continuous real driver gives such a hull family through this [ordinary differential equation](../../../../../ordinary-differential-equation.md). A continuous driver alone need not have a continuous [Loewner trace](../../../../../trace-of-a-loewner-chain.md); that additional assertion is part of the trace theory of [SLE](../../../../../schramm-loewner-evolution.md), not of the deterministic correspondence theorem.

A continuous process $\gamma:[0,\infty)\to\overline{\mathbb H}$ is chordal [Schramm–Loewner evolution](../../../../../schramm-loewner-evolution.md) with parameter $\kappa$ from $0$ to infinity when $\gamma_0=0$, its filled past generates these capacity-$2t$ hulls, and their [Loewner driving function](../../../../../loewner-driving-function.md) is

$$
\boxed{\xi_t=\sqrt\kappa\,B_t,}
$$

with $B$ standard real [Brownian motion](../../../../../brownian-motion-split.md). The filling includes bounded components cut off from infinity. Equivalently its [Loewner trace](../../../../../trace-of-a-loewner-chain.md) is the continuous extension of $\gamma_t=\lim_{y\downarrow0}g_t^{-1}(\xi_t+iy)$. This last [boundary](../../../../../boundary-of-a-set.md) limit is the trace-existence input for [SLE](../../../../../schramm-loewner-evolution.md).

Fix $r>0$ and scale space and time together:

$$
\widehat K_t=r^{-1}K_{r^2t},\qquad
\widehat g_t(z)=r^{-1}g_{r^2t}(rz),\qquad
\widehat\xi_t=r^{-1}\xi_{r^2t}.
$$

The [half-plane capacity](../../../../../half-plane-capacity.md) of $\widehat K_t$ is $2t$ by part (a). Differentiation gives

$$
\partial_t\widehat g_t(z)=\frac2{\widehat g_t(z)-\widehat\xi_t}.
$$

By [Brownian scaling](../../../../../brownian-scaling.md), $r^{-1}B_{r^2t}$ is again standard [Brownian motion](../../../../../brownian-motion-split.md), so the new driver has the same law as the old one. Uniqueness of the [Chordal Loewner equation](../../../../../chordal-loewner-equation.md) transfers this equality to the hulls and their continuous [Loewner traces](../../../../../trace-of-a-loewner-chain.md). Thus

$$
\boxed{(r^{-1}\gamma_{r^2t})_{t\geq0}\ \overset{d}=\ (\gamma_t)_{t\geq0}.}
$$

This is [capacity-parametrized scale invariance of a Loewner chain](../../../../../capacity-parametrized-scale-invariance-of-a-loewner-chain.md). It includes $\kappa=0$, when the driver is zero and the trace is the deterministic vertical slit $\gamma_t=2i\sqrt t$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
