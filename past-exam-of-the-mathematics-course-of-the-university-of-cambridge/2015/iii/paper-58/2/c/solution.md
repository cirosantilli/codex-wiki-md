<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a spherical hydrostatic star with negligible surface [pressure](../../../../../../pressure.md), the [stellar virial theorem](../../../../../../stellar-virial-theorem.md) is

$$
\Omega+3\int P\,dV=0.
$$

For a monatomic nonrelativistic [perfect gas](../../../../../../ideal-gas.md), $U=\tfrac32\int P\,dV$, so $2U+\Omega=0$ and the total energy is $E=U+\Omega=\Omega/2$. Half the released binding energy raises the [internal energy](../../../../../../internal-energy.md); only the other half can be radiated. With fixed mass, no nuclear supply and no external work, [conservation of energy](../../../../../../conservation-of-energy.md) gives

$$
L=-\frac{dE}{dt}=-\frac12\frac{d\Omega}{dt}.
$$

For the [uniform-density stellar model](../../../../../../uniform-density-stellar-model.md), this becomes the contraction-luminosity evolution equation

$$
\boxed{L(t)=-\frac{3GM^2}{10R^2}\frac{dR}{dt},\qquad\frac{d}{dt}\left(\frac1R\right)=\frac{10L(t)}{3GM^2}.}
$$

It relates [luminosity](../../../../../../luminosity.md) to the contraction rate; it does not by itself prescribe $L(t)$. Given $L(t)$,

$$
\frac1{R(t)}=\frac1{R_0}+\frac{10}{3GM^2}\int_0^tL(t')\,dt'.
$$

For constant [luminosity](../../../../../../luminosity.md), $R(t)=R_0/[1+t/t_0]$ with $t_0=3GM^2/(10R_0L)$. This describes quasi-static [Kelvin-Helmholtz contraction](../../../../../../kelvin-helmholtz-mechanism.md), not dynamical free fall. If the gas has a different constant [specific-heat ratio](../../../../../../heat-capacity-ratio.md) $\gamma_g$, the appropriate [stellar virial theorem](../../../../../../stellar-virial-theorem.md) is $3(\gamma_g-1)U+\Omega=0$, so the radiated fraction of binding release is $(3\gamma_g-4)/[3(\gamma_g-1)]$ rather than universally one half.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
