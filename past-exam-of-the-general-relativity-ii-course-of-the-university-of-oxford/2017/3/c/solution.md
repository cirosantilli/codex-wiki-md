<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Reflection across $\theta=\pi/2$ is an [isometry](../../../../isometry.md); a [geodesic](../../../../geodesic.md) initially tangent to its fixed equatorial plane remains in that plane by uniqueness of the [geodesic equation](../../../../geodesic-equation.md). Thus take $\theta=\pi/2$, $\dot\theta=0$, and $\Sigma=r^2$. Define the algebraic abbreviations

$$
A=1-\frac{2M}{r},\qquad
B=\frac{2Ma}{r},\qquad
C=r^2+a^2+\frac{2Ma^2}{r}.
$$

The [conserved quantities](../../../../conserved-quantity.md) of part (b) become

$$
E=A\dot t+B\dot\phi,\qquad
L=-B\dot t+C\dot\phi,
\qquad
AC+B^2=\Delta.
$$

For $\Delta\ne0$, inversion gives

$$
\dot t=\frac{CE-BL}{\Delta},\qquad
\dot\phi=\frac{BE+AL}{\Delta}.
$$

The [null condition](../../../../null-condition.md) can be written without expanding a quadratic square:

$$
0=-E\dot t+L\dot\phi+\frac{r^2}{\Delta}\dot r^2.
$$

Substituting the preceding expressions yields the [equatorial Kerr null geodesic radial equation](../../../../equatorial-kerr-null-geodesic-radial-equation.md)

$$
\boxed{
\dot r^2
=E^2+\frac{a^2E^2-L^2}{r^2}
+\frac{2M(L-aE)^2}{r^3}.
}
$$

An equivalent useful polynomial form is

$$
\boxed{
r^4\dot r^2=\mathcal R(r),\qquad
\mathcal R(r)=\left[E(r^2+a^2)-aL\right]^2
-\Delta(L-aE)^2.
}
$$

These expressions use an [affine parameter](../../../../affine-parameter.md) $s$; a common rescaling of $E$ and $L$ accompanies its rescaling. The inversion was performed in the exterior $r>r_+$, where [Boyer-Lindquist coordinates](../../../../boyer-lindquist-coordinates.md) are regular. The polynomial radial identity has a smooth continuation to a horizon, but the formulas for $\dot t$ and $\dot\phi$ there must be replaced by regular-coordinate expressions. In the limit $a=0$, the result reduces to the [Schwarzschild spacetime](../../../../schwarzschild-spacetime-split.md) equation $\dot r^2=E^2-(1-2M/r)L^2/r^2$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity II course of the University of Oxford](../../../split.md)
5. [General relativity II course of the University of Oxford](../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
