<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use units $c=\hbar=k_B=1$, and write $H=\dot a/a$ for the [Hubble parameter](../../../../../../hubble-parameter.md), with dots denoting [cosmic time](../../../../../../cosmic-time.md). Differentiating the [Friedmann equation](../../../../../../friedmann-equations.md) gives

$$
2H\dot H=\frac{8\pi G}{3}\dot\rho+\frac{2KH}{a^2}.
$$

On an interval where $H\ne0$, use the [Hubble parameter identity](../../../../../../hubble-parameter-identity.md) $\dot H=\ddot a/a-H^2$ and the [Friedmann acceleration equation](../../../../../../friedmann-acceleration-equation.md) to find

$$
\dot H=-4\pi G(\rho+P)+\frac K{a^2}.
$$

Substitution cancels the curvature term and gives the **continuity equation**

$$
\boxed{\dot\rho=-3H(\rho+P).}
$$

The [cosmological perfect-fluid continuity equation](../../../../../../cosmological-perfect-fluid-continuity-equation.md) extends by continuity through a regular isolated turning point. Physically it states that the change of energy in a [comoving volume](../../../../../../comoving-volume.md) is the negative of the pressure work: $d(\rho a^3)=-P\,d(a^3)$.

For [separately conserved cosmological fluids](../../../../../../separately-conserved-cosmological-fluids.md), each component obeys this equation individually. A constant [equation-of-state parameter](../../../../../../equation-of-state-parameter.md) $w_i=P_i/\rho_i$ therefore gives

$$
\frac{d\log\rho_i}{d\log a}=-3(1+w_i),
\qquad \rho_i(a)=\rho_{i,0}a^{-3(1+w_i)},
$$

where the present [scale factor](../../../../../../scale-factor-cosmology.md) is normalized to $a_0=1$. Thus the **component density laws** are

$$
\boxed{\rho_r=\rho_{r,0}a^{-4},\qquad
\rho_m=\rho_{m,0}a^{-3},\qquad
\rho_\Lambda=\rho_{\Lambda,0}.}
$$

The extra factor for [radiation in cosmology](../../../../../../radiation-in-cosmology.md) is the [cosmological redshift](../../../../../../cosmological-redshift.md) of each photon's energy; [pressureless matter](../../../../../../pressureless-matter.md) has only number dilution, while the specified [dark energy](../../../../../../dark-energy.md) is a [cosmological constant](../../../../../../cosmological-constant.md).

The [critical density](../../../../../../critical-density.md) at a given expansion rate is the total density that makes the spatial curvature vanish:

$$
\rho_{\rm crit}(t)=\frac{3H(t)^2}{8\pi G},\qquad
\Omega_i(t)=\frac{\rho_i(t)}{\rho_{\rm crit}(t)}.
$$

These [cosmological density parameters](../../../../../../cosmological-density-parameter.md) use the critical density at that same time. Put $E(a)=H(a)/H_0$ and $\Omega_{K,0}=-K/H_0^2$. The [Friedmann equation](../../../../../../friedmann-equations.md) yields

$$
E(a)^2=\Omega_{r,0}a^{-4}+\Omega_{m,0}a^{-3}
+\Omega_{\Lambda,0}+\Omega_{K,0}a^{-2}.
$$

Consequently the **fractional-density evolution**, rather than just the component-density evolution, is

$$
\boxed{\Omega_r(a)=\frac{\Omega_{r,0}a^{-4}}{E(a)^2},\qquad
\Omega_m(a)=\frac{\Omega_{m,0}a^{-3}}{E(a)^2},\qquad
\Omega_\Lambda(a)=\frac{\Omega_{\Lambda,0}}{E(a)^2}.}
$$

In particular $\sum_i\Omega_i=1+K/(a^2H^2)$. The simple powers of $a$ alone apply to $\rho_i$, or to $\rho_i/\rho_{{\rm crit},0}$, not to the instantaneous [cosmological density parameters](../../../../../../cosmological-density-parameter.md). At a recollapse turning point $H=0$, those instantaneous ratios are undefined even though the component densities remain finite.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
