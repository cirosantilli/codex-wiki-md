<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $D=u_1>0$ denote the front speed in the stationary upstream frame. In the [shock frame](../../../../../../shock-frame.md), the upstream and downstream velocities are $-D$ and $-D/r$. Taking $M_1\to\infty$ in the [Rankine-Hugoniot conditions for a perfect gas](../../../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md) gives

$$
\boxed{\rho_2=\frac{\gamma+1}{\gamma-1}\rho_1,\qquad p_2=\frac{2}{\gamma+1}\rho_1D^2.}
$$

The downstream laboratory velocity is $D-D/r=2D/(\gamma+1)$, which distinguishes the gas speed from the front speed.

For the [planar blast-wave energy scaling](../../../../../../planar-blast-wave-energy-scaling.md) of a [self-similar blast wave](../../../../../../self-similar-blast-wave.md), integration of the total [energy density](../../../../../../energy-density.md) over the shocked interval $0<z<Z$ gives the energy per unit area on this side:

$$
E_+=\int_0^Z\left(\frac{\rho u^2}{2}+\frac{p}{\gamma-1}\right)dz
=\rho_1Z\dot Z^2 I,\qquad
I=\int_0^1\left(\frac12fh^2+\frac{g}{\gamma-1}\right)d\eta.
$$

The [similarity solution](../../../../../../similarity-solution.md) makes $I$ time-independent; a finite positive explosion energy requires $0<I<\infty$. Conservation of energy therefore gives $\dot Z=(E_+/(\rho_1I))^{1/2}Z^{-1/2}$ for the expanding front. Integrating from $Z(0)=0$,

$$
\frac23Z^{3/2}=\left(\frac{E_+}{\rho_1I}\right)^{1/2}t,
\qquad
\boxed{Z(t)=\left(\frac{9}{4I}\right)^{1/3}\left(\frac{E_+}{\rho_1}\right)^{1/3}t^{2/3}.}
$$

If $E$ denotes the one-sided energy, $C=(9/(4I))^{1/3}$. If the released energy $E$ feeds two symmetric fronts, $E_+=E/2$ and $C=(9/(8I))^{1/3}$. **In either convention the requested scaling is $Z=C(E/\rho_1)^{1/3}t^{2/3}$.** The constant depends on the [similarity profiles](../../../../../../similarity-profile.md) and the energy convention; energy conservation determines the exponent without solving those profiles. The [Strong-shock Rankine-Hugoniot conditions](../../../../../../strong-shock-rankine-hugoniot-conditions.md) additionally fix $f(1)=(\gamma+1)/(\gamma-1)$ and $g(1)=h(1)=2/(\gamma+1)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
