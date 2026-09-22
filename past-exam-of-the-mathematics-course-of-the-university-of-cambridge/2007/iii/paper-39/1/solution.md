<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [compact H-hull](../../../../../compact-h-hull.md) is a bounded relatively closed subset $K$ of $\mathbb H$ with [simply connected](../../../../../simply-connected-space.md) complement, considered together with its compact [closure](../../../../../closure-topology.md) in $\overline{\mathbb H}$. Its unique [mapping-out function](../../../../../mapping-out-function-of-a-compact-h-hull.md) has [hydrodynamic normalization at infinity](../../../../../hydrodynamic-normalization-at-infinity.md)

$$
g_K:\mathbb H\setminus K\longrightarrow\mathbb H,
\qquad g_K(z)=z+\frac{a_K}{z}+O(z^{-2})\quad(z\to\infty).
$$

The nonnegative coefficient $a_K$ is its [half-plane capacity](../../../../../half-plane-capacity.md). Thus the [half-plane-capacity parameterization](../../../../../half-plane-capacity-parameterization.md) here gives $g_t(z)=z+2t/z+O(z^{-2})$. Strict increase means $K_s\subsetneq K_t$ whenever $s<t$; the strictly increasing capacity already excludes equality.

The [Loewner local growth property](../../../../../loewner-local-growth-property.md) means that the new growth becomes small after removing the old [compact H-hull](../../../../../compact-h-hull.md). More precisely set $K_{t,t+h}=\overline{g_t(K_{t+h}\setminus K_t)}$, taking the [closure](../../../../../closure-topology.md) from the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md). On each bounded time interval, the diameters of these image [compact H-hulls](../../../../../compact-h-hull.md) tend uniformly to zero as $h\downarrow0$. Equivalently the new growth can be separated from infinity by [crosscuts](../../../../../crosscut.md) of vanishing diameter in the mapped domain. It is this single-point local growth, together with capacity continuity, that gives a continuous real [Loewner driver](../../../../../loewner-driving-function.md).

The [Loewner transform](../../../../../loewner-driving-function.md) $\xi_t$ is the limiting point at which this mapped growth occurs:

$$
\boxed{\xi_t=\lim_{h\downarrow0}g_t(z_h),\qquad z_h\in(K_{t+h}\setminus K_t)\cap\mathbb H.}
$$

The limit is independent of the chosen new-growth points. The [Loewner correspondence theorem](../../../../../loewner-correspondence-theorem.md) says that the resulting [mapping-out functions](../../../../../mapping-out-function-of-a-compact-h-hull.md) satisfy

$$
\partial_tg_t(z)=\frac{2}{g_t(z)-\xi_t},\qquad g_0(z)=z.
$$

Conversely, given a continuous real $\xi$, solve this [ordinary differential equation](../../../../../ordinary-differential-equation.md) until the maximal lifetime $T_z$ of each $z\in\mathbb H$. The surviving set $H_t=\{z:T_z>t\}$ is mapped conformally onto $\mathbb H$ by $g_t$; its complement, with the appropriate [boundary](../../../../../boundary-of-a-set.md) [closure](../../../../../closure-topology.md), is $K_t$. The [Laurent coefficient](../../../../../laurent-coefficient.md) is $2t$, and the composition law reconstructs the local growth. A continuous [Loewner driver](../../../../../loewner-driving-function.md) always determines the [compact H-hulls](../../../../../compact-h-hull.md); generation by a continuous [Loewner trace](../../../../../trace-of-a-loewner-chain.md) is an additional property, not a conclusion for every continuous [Loewner driver](../../../../../loewner-driving-function.md).

A chordal [SLE](../../../../../schramm-loewner-evolution.md) [Loewner trace](../../../../../trace-of-a-loewner-chain.md) in the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md) with parameter $\kappa\geq0$ is the continuous curve associated with the [Loewner driver](../../../../../loewner-driving-function.md) $\xi_t=\sqrt\kappa B_t$, where $B$ is standard real [Brownian motion](../../../../../brownian-motion-split.md) started at zero. It starts at zero, its [compact H-hull](../../../../../compact-h-hull.md) at time $t$ is the curve's past with all pockets cut off from infinity filled, and

$$
\gamma(t)=\lim_{y\downarrow0}g_t^{-1}(\xi_t+iy).
$$

The capacity clock has $\operatorname{hcap}(K_t)=2t$. For $\kappa=0$ this gives the vertical slit $\gamma(t)=2i\sqrt t$.

To prove [Scaling invariance of SLE](../../../../../scaling-invariance-of-sle.md), fix $r>0$ and put

$$
\widehat K_t=r^{-1}K_{r^2t},\qquad
\widehat g_t(z)=r^{-1}g_{r^2t}(rz),\qquad
\widehat\xi_t=r^{-1}\xi_{r^2t}.
$$

The [Laurent series](../../../../../laurent-series.md) of $\widehat g_t$ has coefficient $2t$, and direct differentiation gives

$$
\partial_t\widehat g_t(z)=\frac2{\widehat g_t(z)-\widehat\xi_t}.
$$

[Brownian scaling](../../../../../brownian-scaling.md) says $(r^{-1}B_{r^2t})_{t\geq0}$ has the same law as $B$. The [Loewner drivers](../../../../../loewner-driving-function.md) therefore agree in law, and uniqueness of the [Chordal Loewner equation](../../../../../chordal-loewner-equation.md) gives equality in law of the maps, [compact H-hulls](../../../../../compact-h-hull.md), and continuous [Loewner traces](../../../../../trace-of-a-loewner-chain.md):

$$
\boxed{(r^{-1}\gamma(r^2t))_{t\geq0}\overset d=(\gamma(t))_{t\geq0}.}
$$

This identifies the time change $t\mapsto r^2t$ as well as the spatial scaling.

For a [simply connected](../../../../../simply-connected-space.md) [Jordan domain](../../../../../jordan-domain.md) $D$ with distinct marked [boundary](../../../../../boundary-of-a-set.md) points, choose a [conformal bijection](../../../../../biholomorphism.md) $f:\mathbb H\to D$ taking zero to the initial point and infinity to the target, and use $f(\gamma)$ as an unparameterized curve. The [Caratheodory boundary extension theorem](../../../../../caratheodory-boundary-extension-theorem.md) supplies the [boundary](../../../../../boundary-of-a-set.md) values of $f$. Any second such map is $f\circ(z\mapsto rz)$ for $r>0$, because the automorphisms of $\mathbb H$ fixing zero and infinity are positive dilations. The [Scaling invariance of SLE](../../../../../scaling-invariance-of-sle.md) just proved makes the two image laws identical, up to the corresponding deterministic change of capacity clock. Thus this defines [SLE](../../../../../schramm-loewner-evolution.md) consistently in marked [Jordan domains](../../../../../jordan-domain.md). The assumed $|\gamma(t)|\to\infty$ and the continuous [boundary](../../../../../boundary-of-a-set.md) extension give $f(\gamma(t))\to f(\infty)$, the specified target. The law is conformally natural and does not impose a distinguished [half-plane-capacity parameterization](../../../../../half-plane-capacity-parameterization.md) on an arbitrary domain.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
