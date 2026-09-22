<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

A [thermodynamic potential](../../../../../thermodynamic-potential-split.md) packages the equilibrium state in variables suited to the imposed constraints. For a simple fluid, $U(S,V,N)$ has differential $dU=T\,dS-p\,dV+\mu\,dN$. [Legendre transforms](../../../../../convex-conjugate.md) give $H=U+pV$, $F=U-TS$ and $G=U+pV-TS$, with [natural variables of a thermodynamic potential](../../../../../natural-variables-of-a-thermodynamic-potential.md) $(S,p,N)$, $(T,V,N)$ and $(T,p,N)$ respectively. At fixed [particle number](../../../../../particle-number.md), **[Helmholtz free energy](../../../../../helmholtz-free-energy.md) is minimized at fixed $T,V$; [Gibbs free energy](../../../../../gibbs-free-energy.md) at fixed $T,p$**.

A flow vessel is an open [control volume](../../../../../control-volume.md), even if its walls are enclosed. For each inlet, [pressure](../../../../../pressure-split.md) forces carry flow [work](../../../../../work.md) $p\,dV$ in addition to [internal energy](../../../../../internal-energy-split.md). The steady first-law balance is

$$
\sum_{\rm in}\dot m(h+v^2/2+gz)+\dot Q-\dot W_{\rm shaft}
=\sum_{\rm out}\dot m(h+v^2/2+gz).
$$

With no [heat](../../../../../heat-split.md) exchange, shaft [work](../../../../../work.md), or significant kinetic and gravitational [energy](../../../../../energy-split.md) differences, the [enthalpy](../../../../../enthalpy-split.md) fluxes are equal. [Mass](../../../../../mass.md) flow must also balance. This equality concerns mass-flow-weighted specific enthalpies, not an unweighted sum over pipes.

Use the [liquefaction yield with separate warm-gas and liquid outlets](../../../../../liquefaction-yield-with-separate-warm-gas-and-liquid-outlets.md). The wording specifies that the outgoing gas is at 14 K; it does not require the outgoing [liquid](../../../../../liquid.md) to have that [temperature](../../../../../temperature-split.md). The two outlet streams need not be in mutual [thermal equilibrium](../../../../../thermal-equilibrium-split.md). Taking $H$ as the printed [specific enthalpy](../../../../../specific-enthalpy.md), the [steady-flow energy balance](../../../../../steady-flow-energy-balance.md) gives

$$
H(p)=\alpha H_\ell+(1-\alpha)H(p_0),\qquad
\boxed{\alpha=\frac{H(p_0)-H(p)}{H(p_0)-H_\ell}.}
$$

For fixed outlet enthalpies the greatest yield occurs at the smallest inlet [enthalpy](../../../../../enthalpy-split.md). **Among the tabulated [pressures](../../../../../pressure-split.md) this is 30 atm.** Approximating the atmospheric-pressure gas [enthalpy](../../../../../enthalpy-split.md) by the tabulated zero-pressure limiting value gives

$$
\boxed{\alpha\simeq\frac{8.74-7.18}{8.74-1.01}=0.202,\quad p\simeq30\,\mathrm{atm}.}
$$

This uses a low-pressure approximation: $p_0=1$ atm is not literally the zero-pressure table entry. Linear interpolation to 1 atm would instead give $H(p_0)\simeq8.651\times10^4\,\mathrm{J\,kg^{-1}}$ and $\alpha\simeq0.193$. The sparse table does not determine an exact continuous optimum between entries.

Atmospheric-pressure liquid [helium](../../../../../helium.md) must be much colder than the 14 K gas outlet: its normal boiling point is about 4.224 K.[Helium-4 characteristic-property table: normal boiling point 4.224 K](../../../../../index-of-semiconductor-process-gases-helium-by-national-institute-of-standards-and-technology.md) A [counterflow heat exchanger](../../../../../counterflow-heat-exchanger.md) can return cold gas through the incoming stream before that gas leaves the overall [control volume](../../../../../control-volume.md), while the collected [liquid](../../../../../liquid.md) leaves separately at the cold end. This is a possible interpretation of the whole apparatus, rather than an extra diagram specified by the question. The enthalpy calculation needs only the stated inlet and outlet properties; it does not assume one equilibrium vessel containing both phases at 14 K. In particular, $H(p_0)-H_\ell$ is an outlet-stream enthalpy difference, not the [latent heat](../../../../../latent-heat.md) of vaporization at one common [temperature](../../../../../temperature-split.md).

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
