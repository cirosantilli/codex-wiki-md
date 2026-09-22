<h1 id="36d/solution">Solution</h1>

↑ **Parent:** [36D](../36d.md)

Set $f(r)=1-2M/r$ and use [proper time](../../../../../proper-time.md) along a timelike [geodesic](../../../../../geodesic.md). In the equatorial plane, the radial [Christoffel symbols](../../../../../christoffel-symbol.md) needed for a circular orbit are

$$
\Gamma^r_{tt}=\frac12ff'=\frac{fM}{r^2},\qquad\Gamma^r_{\varphi\varphi}=-fr.
$$

The radial [geodesic equation](../../../../../geodesic-equation.md) with $\dot r=0$ gives $(fM/r^2)\dot t^2-fr\dot\varphi^2=0$. Outside the horizon this implies

$$
\boxed{\left(\frac{d\varphi}{dt}\right)^2=\frac{M}{r^3}.}
$$

For stability use the conserved energy $E=f\dot t$ and [angular momentum](../../../../../angular-momentum.md) $L=r^2\dot\varphi$. The normalization of the timelike tangent in the [Schwarzschild metric](../../../../../schwarzschild-spacetime.md) gives $\dot r^2+V(r)=E^2$, with the [effective potential for timelike Schwarzschild geodesics](../../../../../effective-potential-for-timelike-schwarzschild-geodesics.md)

$$
V(r)=f(r)\left(1+\frac{L^2}{r^2}\right).
$$

At a circular orbit $V'=0$, so $L^2=Mr^2/(r-3M)$, requiring $r>3M$. Differentiate $V$ holding this conserved $L$ fixed and then substitute the circular value:

$$
V''(r)=\frac{2M(r-6M)}{r^3(r-3M)}.
$$

The linear radial perturbation equation is $\delta\ddot r=-V''(r)\delta r/2$. Thus **circular timelike orbits are stable for $r>6M$**, unstable for $3M<r<6M$, with the marginal case at $6M$.

For the orbiting astronaut at radius $R$, use $d\varphi/dt=\sqrt{M/R^3}$ to obtain

$$
\frac{d\tau_a}{dt}=\sqrt{1-\frac{2M}{R}-R^2\left(\frac{d\varphi}{dt}\right)^2}=\sqrt{1-\frac{3M}{R}}.
$$

The static Earth twin has $d\tau_0/dt=\sqrt{1-2M/R_0}$. During equal coordinate-time intervals of the long circular-orbit phase, the astronaut ages less precisely when

$$
1-\frac{3M}{R}<1-\frac{2M}{R_0}\quad\Longleftrightarrow\quad\boxed{2R<3R_0.}
$$

The outward and return transfers have finite additional proper times; the stated long-orbit comparison is the limit in which the circular phase dominates them. At equality the circular phase contributes no age difference, so transfer details can decide the finite-trip result.

## ↑ Ancestors (10)

1. [36D](../36d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
