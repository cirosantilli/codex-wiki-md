<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In a [parallel-plate rheometer](../../../../../../parallel-plate-rheometer.md), a point at radius $r$ on the upper plate moves at speed $\Omega r$. The thin-gap approximation therefore gives the local [shear rate](../../../../../../shear-rate.md)

$$
\dot\gamma(r)=\frac{\Omega r}{h}.
$$

Define the rim value

$$
\dot\gamma_R=\frac{\Omega R}{h},
\qquad
\dot\gamma(r)=\dot\gamma_R\frac rR.
$$

An annulus of radius $r$ and width $dr$ has area $2\pi r\,dr$; its tangential force is $\tau(r)2\pi r\,dr$, and its moment arm is $r$. The measured [torque](../../../../../../torque.md) is consequently

$$
T=2\pi\int_0^R\tau(\dot\gamma(r))r^2\,dr.
$$

For a [generalized Newtonian fluid](../../../../../../generalized-newtonian-fluid.md), $\tau=\eta(\dot\gamma)\dot\gamma$. Changing the integration variable from $r$ to $\dot\gamma$ gives

$$
\boxed{
T=\frac{2\pi R^3}{\dot\gamma_R^3}
\int_0^{\dot\gamma_R}\eta(\dot\gamma)\dot\gamma^3\,d\dot\gamma}.
$$

Thus the requested kernel is

$$
f(\dot\gamma,R,\dot\gamma_R)
=\frac{2\pi R^3\dot\gamma^3}{\dot\gamma_R^3}.
$$

Multiplying by $\dot\gamma_R^3$ and taking a [derivative](../../../../../../derivative.md) with respect to $\dot\gamma_R$ turns the upper-limit contribution of the [integral](../../../../../../integral.md) into the rim viscosity:

$$
\frac{d}{d\dot\gamma_R}\left(T\dot\gamma_R^3\right)
=2\pi R^3\eta(\dot\gamma_R)\dot\gamma_R^3.
$$

Therefore

$$
\boxed{
\eta(\dot\gamma_R)
=\frac{3T+\dot\gamma_R\,dT/d\dot\gamma_R}
{2\pi R^3\dot\gamma_R}
=\frac{3T+\Omega\,dT/d\Omega}
{2\pi R^3\dot\gamma_R}}.
$$

A measured torque curve and its slope hence determine $\eta$ over the range of imposed rim shear rates.

The experimental law implies

$$
\dot\gamma_R=\frac{\Omega R}{h}=\alpha(T-T_c),
\qquad
T=T_c+\frac{\dot\gamma_R}{\alpha}.
$$

Substitution gives

$$
\boxed{
\eta(\dot\gamma)
=\frac{3T_c}{2\pi R^3\dot\gamma}
+\frac{2}{\pi\alpha R^3}}.
$$

The graph is a decreasing rectangular hyperbola with a positive high-rate plateau $2/(\pi\alpha R^3)$ and a $1/\dot\gamma$ divergence at the origin. Equivalently,

$$
\tau=\eta\dot\gamma
=\frac{3T_c}{2\pi R^3}
+\frac{2}{\pi\alpha R^3}\dot\gamma,
$$

so the inferred material is a [Bingham plastic](../../../../../../bingham-plastic.md) with yield stress $3T_c/(2\pi R^3)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
