<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For constant [buoyancy frequency](../../../../../../buoyancy-frequency.md) in the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), the ambient density is

$$
\rho_a(z)=\rho_0\left(1-\frac{N^2z}{g}\right).
$$

Conservation of liquid mass during [fluid entrainment](../../../../../../fluid-entrainment.md) gives $d(V\rho)/dz=\rho_a(z)V'(z)$, with $\rho(0)=\rho_0$. Integrating by parts,

$$
V(z)[\rho(z)-\rho_a(z)]=\frac{\rho_0N^2}{g}\int_0^zV(s)ds.
$$

Since $a=a_0+\alpha z$ and $V\propto a^3$,

$$
\frac1V\int_0^zV(s)ds=\frac{a^4-a_0^4}{4\alpha a^3}.
$$

Hence the water density within the thermal is

$$
\boxed{\rho(z)=\rho_0\left[1-\frac{N^2z}{g}
+\frac{N^2(a^4-a_0^4)}{4\alpha g a^3}\right].}
$$

The entrained water is denser than its new surroundings because it retains a mixture of fluid drawn from lower levels.

The bulk density is $\rho(1-\phi)$. Dropping products of the small density contrast with $\phi$, its net [reduced gravity](../../../../../../reduced-gravity-split.md) is

$$
\boxed{g'(z)=\frac1{a^3}\left[\frac{g\phi_0a_0^3}{1-z/H_p}
-\frac{N^2}{4\alpha}(a^4-a_0^4)\right].}
$$

The first term is the expanding-bubble contribution and the second is the restoring effect of stratification. In the quasi-steady Froude model, ascent stops when $g'=0$. The [neutral height of a bubbly thermal in a stratified fluid](../../../../../../neutral-height-of-a-bubbly-thermal-in-a-stratified-fluid.md) therefore satisfies

$$
\boxed{(1-z/H_p)\left[(a_0+\alpha z)^4-a_0^4\right]
-\frac{4\alpha g\phi_0a_0^3}{N^2}=0.}
$$

This is a fifth-degree polynomial, with leading coefficient $-\alpha^4/H_p$ at finite release pressure. The relevant height is the first positive zero reached while the thermal is still below the surface, dilute and within the Boussinesq range. Depending on parameters there may be no such zero before the surface, or more than one mathematical zero; a later root beyond a first stopping point is not another continuous ascent solution. The model's stopping height is a neutral-buoyancy estimate, not a claim that inertial overshoot is absent.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
