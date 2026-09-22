<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $r_s\gg d_H$, a regular adiabatic perturbation follows the large-scale [density contrast](../../../../density-contrast.md) growth in [b](../b.md); this does not require causal communication across the perturbation. Since $d_H=c/H$, the [Friedmann equation](../../../../friedmann-equations.md) gives $d_H\propto a^2$ during [radiation domination](../../../../radiation-domination.md) and $d_H\propto a^{3/2}$ during [matter domination](../../../../matter-domination.md). A fixed comoving perturbation has physical size $r_s=aR$, so its ratio to $d_H$ decreases as $a^{-1}$ or $a^{-1/2}$ until [cosmological horizon entry](../../../../cosmological-horizon-entry.md).

**The numerical “exactly at equality” assertion is inconsistent with the supplied parameters and $d_H=c/H$.** Normalize $a_0=1$ and use the supplied $\Omega_\gamma$ as the whole radiation component. Then

$$
a_{\rm eq}=\frac{\Omega_\gamma}{\Omega_m}=\frac1{3000},\qquad
H^2=H_0^2\left(\Omega_\gamma a^{-4}+\Omega_ma^{-3}\right).
$$

Both terms must be retained at [matter-radiation equality](../../../../matter-radiation-equality.md). The present comoving size corresponding to its [Hubble radius](../../../../hubble-radius.md) is

$$
\boxed{R_{H,\rm eq}=\frac{c}{a_{\rm eq}H_{\rm eq}}
=\frac{c}{H_0}\frac{\sqrt{\Omega_\gamma}}{\sqrt2\,\Omega_m}=106.4\ \mathrm{Mpc}.}
$$

Its physical size then is $0.0355\ \mathrm{Mpc}$. A mode with $R=79\ \mathrm{Mpc}$ has physical size only $0.0263\ \mathrm{Mpc}$ at equality, already inside the [Hubble radius](../../../../hubble-radius.md). More explicitly, putting $q=RH_0/c$ in $aR=c/H(a)$ gives

$$
a_{\rm ent}=\frac{q^2\Omega_m+\sqrt{q^4\Omega_m^2+4q^2\Omega_\gamma}}2
=2.27\times10^{-4}=0.681a_{\rm eq}.
$$

This is a direct numerical counterexample using the stated data. Neglecting one component exactly at equality instead gives $150.5\ \mathrm{Mpc}$, which also does not produce $79\ \mathrm{Mpc}$. Late-time dark energy is negligible at these early times.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
