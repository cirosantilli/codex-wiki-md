<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [WKB approximation](../../../../../../wkb-approximation.md) treats the vertical [wavenumber](../../../../../../wavenumber.md) as locally constant over one vertical [wavelength](../../../../../../wavelength.md). Write $w=\Re\{A(z)e^{ikx+i\int^z m(s)ds}\}$, with $|m'|\ll m^2$ and $|A'|\ll |mA|$. For the [stationary internal-wave WKB solution](../../../../../../stationary-internal-wave-wkb-solution.md), $A\propto m^{-1/2}$ away from singular or turning levels. A small terrain slope and small perturbations are also needed for [Linearized Boussinesq equations](../../../../../../linearized-boussinesq-equations.md).

Let $p$ be the perturbation [fluid pressure](../../../../../../fluid-pressure.md) divided by reference [mass density](../../../../../../density.md), and $b$ the [buoyancy perturbation](../../../../../../buoyancy-perturbation.md). The steady [Linearized Boussinesq equations](../../../../../../linearized-boussinesq-equations.md) and [incompressibility condition](../../../../../../incompressible-flow.md) are

$$
Uu_x+U'w=-p_x,\qquad Uw_x=-p_z+b,\qquad Ub_x+N^2w=0,\qquad u_x+w_z=0.
$$

For an $e^{ikx}$ component, elimination gives $u=-w'/(ik)$, $b=-N^2w/(ikU)$ and $p=(Uw'-U'w)/(ik)$. Substitution into vertical momentum gives the exact stationary [Taylor–Goldstein equation](../../../../../../taylor-goldstein-equation.md)

$$
w''+\left(\frac{N^2}{U^2}-\frac{U''}{U}-k^2\right)w=0.
$$

The leading [WKB approximation](../../../../../../wkb-approximation.md) therefore identifies

$$
\boxed{m^2=\frac{N^2}{U^2}-\frac{U''}{U}-k^2=\left(\frac{N^2}{k^2U^2}-\frac{U''}{k^2U}-1\right)k^2.}
$$

The [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) fixes the horizontal [wavenumber](../../../../../../wavenumber.md) to $k=k_T$ for the sinusoidal forcing.

For explicit heights assume a constant positive [buoyancy frequency](../../../../../../buoyancy-frequency.md) $N$, $0<kU_0<N$, and $|S|/N\ll1$. The latter is a large [gradient Richardson number](../../../../../../gradient-richardson-number.md). The [linear shear flow](../../../../../../linear-shear-flow.md) has $U''=0$, so the propagation condition is $|U|<N/k$.

For $S<0$, the first obstruction is the [critical level of an internal gravity wave](../../../../../../critical-level-of-an-internal-gravity-wave.md) at

$$
\boxed{z_c=\frac{U_0}{|S|}.}
$$

As $z\uparrow z_c$, $m\sim N/U\to\infty$. The [critical-height approach of a stationary wave in linear shear](../../../../../../critical-height-approach-of-a-stationary-wave-in-linear-shear.md) has upward [group velocity](../../../../../../group-velocity.md) $c_{gz}\sim kU^2/N$, so the travel time to $z_c$ diverges: the height is a supremum, approached in the ideal ray model. Here $|m'|/m^2\to |S|/N$, which can remain small; it would be incorrect to say that the short-[wavelength](../../../../../../wavelength.md) [WKB approximation](../../../../../../wkb-approximation.md) necessarily fails solely because $m$ diverges. Nevertheless $w\propto U^{1/2}$ and [displacement](../../../../../../displacement.md) $w/(ikU)\propto U^{-1/2}$, so a finite disturbance eventually violates linearity. Dissipation and overturning also matter near this singular level.

For $S>0$, the [turning height of a stationary wave in linear shear](../../../../../../turning-height-of-a-stationary-wave-in-linear-shear.md) is

$$
\boxed{z_t=\frac{N/k-U_0}{S}.}
$$

At $z_t$, $m=0$ and the [WKB approximation](../../../../../../wkb-approximation.md) fails. An [Airy function](../../../../../../airy-function.md) matching region describes reflection and an upper [evanescent wave](../../../../../../evanescent-wave.md). Thus $z_t$ is the highest height of vertical propagation, rather than a sharp cut-off of every disturbance.

The problem initially allows $N(z)$ to vary. Without the extra constant-$N$ assumption, replace the explicit turning height by the first root of $N(z)=k|U_0+Sz|$ encountered on a propagating branch. A declining $N(z)$ can cause a turning level before the negative-shear critical level. **The two closed-form heights require the stated constant-stratification assumption.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 330](../../../paper-330-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
