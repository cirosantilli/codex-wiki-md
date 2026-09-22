<h1 id="36d/solution">Solution</h1>

↑ **Parent:** [36D](../36d.md)

Put $h(r)=1-\mu/r^2$. For the equatorial [geodesic](../../../../../geodesic.md), the [geodesic](../../../../../geodesic.md) [Lagrangian](../../../../../lagrangian.md) is $\mathcal L=\tfrac12[-h\dot t^2+h^{-1}\dot r^2+r^2\dot\phi^2]$, where dots denote [derivatives](../../../../../derivative.md) with respect to the [affine parameter](../../../../../affine-parameter.md). The cyclic coordinates $t,\phi$ give constants $p_t=-h\dot t=-E$ and $p_\phi=r^2\dot\phi=L$. A third constant is the tangent [norm](../../../../../norm.md) $g_{ab}\dot x^a\dot x^b=-\kappa$, preserved by the [geodesic](../../../../../geodesic.md) equation and [metric compatibility](../../../../../metric-compatibility.md). For a timelike [geodesic](../../../../../geodesic.md) rescale the [affine parameter](../../../../../affine-parameter.md) to [proper time](../../../../../proper-time.md) so $\kappa=1$; for a null [geodesic](../../../../../geodesic.md) $\kappa=0$.

Substitute $\dot t=E/h$, $\dot\phi=L/r^2$ into the [norm](../../../../../norm.md) identity and multiply by $h$. It gives the [effective potential](../../../../../effective-potential.md) equation

$$
\boxed{\frac12\dot r^2+V(r)=\frac12E^2,\qquad
V(r)=\frac12\left(1-\frac\mu{r^2}\right)\left(\kappa+\frac{L^2}{r^2}\right)}.
$$

Outside the horizon $r=\sqrt\mu$, its [derivative](../../../../../derivative.md) is $V'=-(L^2-\kappa\mu)/r^3+2\mu L^2/r^5$. A nontrivial circular null [geodesic](../../../../../geodesic.md) requires $L\ne0$, giving

$$
\boxed{r_{\rm null}=\sqrt{2\mu},\qquad V''(r_{\rm null})=-\frac{L^2}{2\mu^2}<0}.
$$

For a circular timelike [geodesic](../../../../../geodesic.md),

$$
\boxed{r_{\rm time}^2=\frac{2\mu L^2}{L^2-\mu},\qquad L^2>\mu}.
$$

At it $V''=-4\mu L^2/r^6<0$, and its radius exceeds $\sqrt{2\mu}$. If $L^2\le\mu$ no finite circular timelike radius exists. Thus **all finite circular null and timelike orbits in this five-dimensional exterior are radially unstable**. The [energy](../../../../../energy.md) of a circular orbit is fixed by $E^2=2V(r)$, not independently arbitrary.

For comparison, with four-dimensional Schwarzschild horizon radius $r_s$, the photon circle is at $3r_s/2$ and is unstable. Circular timelike orbits exist for $r>3r_s/2$; they are unstable below $3r_s$, marginal at $3r_s$ and stable above $3r_s$. The five-dimensional potential has no corresponding stable outer circular timelike branch.

## ↑ Ancestors (10)

1. [36D](../36d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
