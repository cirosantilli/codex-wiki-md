<h1 id="30c/solution">Solution</h1>

↑ **Parent:** [30C](../30c.md)

For $t>0$, the three-dimensional [Kirchhoff formula](../../../../../kirchhoff-formula.md) with zero displacement is

$$
\boxed{u(t,x)=\frac1{4\pi t}\int_{|y-x|=t}g(y)\,dS_y
=\frac t{4\pi}\int_{S^2}g(x+t\omega)\,d\omega}.
$$

The [Strong Huygens principle](../../../../../strong-huygens-principle.md) says that the value depends only on the initial velocity on the sphere of radius $t$, not on points strictly inside it. In particular a compactly supported disturbance leaves no tail at a [fixed point](../../../../../fixed-point.md) after the sphere has passed the support.

For [method of descent for the wave equation](../../../../../method-of-descent-for-the-wave-equation.md), extend the two-dimensional initial velocity independently of the third coordinate. Projecting the three-dimensional sphere onto its planar disk gives two sheets, each with area element $t\,dy/\sqrt{t^2-|y-x|^2}$. Therefore

$$
\boxed{u(t,x)=\frac1{2\pi}\int_{|y-x|<t}
\frac{g(y)}{\sqrt{t^2-|y-x|^2}}\,dy}.
$$

The local argument can use [compact](../../../../../compact-space.md) cutoffs in the extra coordinate, so global Schwartz decay there is unnecessary. The [weak Huygens principle](../../../../../weak-huygens-principle.md) is [finite propagation speed](../../../../../finite-propagation-speed.md): only data in the closed disk of radius $t$ can influence the point. Unlike the three-dimensional free equation, the full interior contributes and a tail can persist.

For the equation with potential $|x|^2$, multiply by $u_t$ and use the product rule:

$$
\partial_t\left[\tfrac12(u_t^2+|\nabla u|^2+|x|^2u^2)\right]
-\nabla\cdot(u_t\nabla u)=u_t(u_{tt}-\Delta u+|x|^2u)=0.
$$

This is the claimed local [energy](../../../../../energy.md) conservation with flux $p=-u_t\nabla u$.

Fix $(t_0,x_0)$ and let $E(t)$ be the integral of $e$ over the shrinking ball $|x-x_0|\le t_0-t$, $0\le t\le t_0-a$ with $a>0$. Its boundary moves inward at speed one. The [divergence theorem](../../../../../divergence-theorem.md) gives

$$
E'(t)=\int_{\partial B}(u_t\partial_\nu u-e)\,dS\le0,
$$

because the negative integrand is

$$
-\tfrac12(u_t-\partial_\nu u)^2
-\tfrac12|\nabla_{\rm tan}u|^2-\tfrac12|x|^2u^2.
$$

All initial data are zero, so $E(0)=0$. Nonnegativity then forces $E(t)=0$. Letting the small terminal ball approach the cone tip proves $u=0$ there; alternatively $u_t=0$ throughout the cone and the initial value fixes $u$. The same argument applied to a difference of solutions whose data agree on the initial ball proves local domain of dependence. Thus **the potential equation has propagation speed at most one and satisfies the [weak Huygens principle](../../../../../weak-huygens-principle.md)**, without requiring finite total [energy](../../../../../energy.md) on all space. It does not assert the strong no-tail property.

## ↑ Ancestors (10)

1. [30C](../30c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
