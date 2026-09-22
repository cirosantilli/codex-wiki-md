<h1 id="9d/solution">Solution</h1>

↑ **Parent:** [9D](../9d.md)

The [Hubble parameter](../../../../../hubble-parameter.md) is the fractional expansion rate

$$
H=\frac{\dot a}{a}.
$$

Here $\rho$ is the homogeneous energy density, $k\in\{-1,0,1\}$ records the sign of the [spatial curvature of an FLRW universe](../../../../../spatial-curvature-of-an-flrw-universe.md), and $R$ is the fixed curvature length scale used with the dimensionless scale factor $a(t)$.

Energy-momentum conservation in a homogeneous expanding universe gives the continuity equation

$$
\dot\rho+3H(\rho+P)=0.
$$

Differentiate the [Friedmann equation](../../../../../friedmann-equations.md)

$$
H^2=\frac{8\pi G}{3c^2}
\left(\rho-\frac{kc^2}{R^2a^2}\right).
$$

Using $\dot a/a=H$ and the continuity equation gives

$$
\dot H
=-\frac{4\pi G}{c^2}(\rho+P)
+\frac{8\pi G}{3c^2}\frac{kc^2}{R^2a^2}.
$$

Eliminating the curvature term with the Friedmann equation yields

$$
\dot H+H^2
=-\frac{4\pi G}{3c^2}(\rho+3P).
$$

Since $\dot H+H^2=\ddot a/a$, this is the [Raychaudhuri equation](../../../../../friedmann-acceleration-equation.md)

$$
\boxed{\frac{\ddot a}{a}
=-\frac{4\pi G}{3c^2}(\rho+3P)}.
$$

Under the [strong energy condition](../../../../../strong-energy-condition.md) $\rho+3P\ge0$, one has $\ddot a\le0$. Thus $a(t)$ is concave, and for $t<t_0$ it lies below its tangent at the present time:

$$
a(t)\le a(t_0)+\dot a(t_0)(t-t_0)
=a(t_0)\bigl[1-H_0(t_0-t)\bigr].
$$

The right side vanishes at $t=t_0-H_0^{-1}$. A positive scale factor therefore cannot extend regularly to that time; it must reach the [Big Bang](../../../../../big-bang.md) singularity at some $t_{\rm BB}\ge t_0-H_0^{-1}$. Equivalently,

$$
\boxed{t_0-t_{\rm BB}\le H_0^{-1}}.
$$

## ↑ Ancestors (10)

1. [9D](../9d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
