<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

For a simple compressible one-component equilibrium system, the fundamental thermodynamic relation is

$$
dU=T\,dS-p\,dV+\mu\,dN.
$$

The [internal energy](../../../../../internal-energy-split.md) has natural variables $(S,V,N)$: its [derivatives](../../../../../derivative.md) give $T$, $-p$ and [chemical potential](../../../../../chemical-potential-split.md) $\mu$. The [natural variables of a thermodynamic potential](../../../../../natural-variables-of-a-thermodynamic-potential.md) identify the independent arguments whose conjugates appear directly in a potential's differential. A [Legendre transform](../../../../../convex-conjugate.md) exchanges a variable for its conjugate, giving potentials suited to different controlled conditions:

| potential | definition | natural variables | differential |
| --- | --- | --- | --- |
| [internal energy](../../../../../internal-energy-split.md) | $U$ | $S,V,N$ | $dU=T\,dS-p\,dV+\mu\,dN$ |
| [enthalpy](../../../../../enthalpy-split.md) | $H=U+pV$ | $S,p,N$ | $dH=T\,dS+V\,dp+\mu\,dN$ |
| [Helmholtz free energy](../../../../../helmholtz-free-energy.md) | $F=U-TS$ | $T,V,N$ | $dF=-S\,dT-p\,dV+\mu\,dN$ |
| [Gibbs free energy](../../../../../gibbs-free-energy.md) | $G=U+pV-TS$ | $T,p,N$ | $dG=-S\,dT+V\,dp+\mu\,dN$ |

For fixed composition and the appropriate closed-system constraints, equilibrium minimizes $U$ at fixed $S,V$, $H$ at fixed $S,p$, $F$ at fixed $T,V$, or $G$ at fixed $T,p$, with other allowable internal variations understood. [Enthalpy](../../../../../enthalpy-split.md) is useful for constant-pressure [heat](../../../../../heat-split.md) exchange with only [pressure](../../../../../pressure-split.md)–volume [work](../../../../../work.md). [Helmholtz free energy](../../../../../helmholtz-free-energy.md) is suited to fixed-temperature, fixed-volume systems, and [Gibbs free energy](../../../../../gibbs-free-energy.md) to fixed-temperature, fixed-pressure phase or chemical equilibrium. Coexisting phases of one substance have equal [chemical potentials](../../../../../chemical-potential-split.md).

Where a potential is twice continuously differentiable, equality of mixed [derivatives](../../../../../derivative.md) gives [Maxwell relations](../../../../../maxwell-relations.md). At fixed $N$, the four usual forms are

$$
\boxed{\left(\frac{\partial T}{\partial V}\right)_S
=-\left(\frac{\partial p}{\partial S}\right)_V,
\qquad
\left(\frac{\partial T}{\partial p}\right)_S
=\left(\frac{\partial V}{\partial S}\right)_p,}
$$



$$
\boxed{\left(\frac{\partial S}{\partial V}\right)_T
=\left(\frac{\partial p}{\partial T}\right)_V,
\qquad
\left(\frac{\partial S}{\partial p}\right)_T
=-\left(\frac{\partial V}{\partial T}\right)_p.}
$$

The fixed subscripts and signs follow from the chosen natural variables. [Derivatives](../../../../../derivative.md) through a nonsmooth phase boundary require separate phase descriptions rather than automatic use of the smooth single-phase formulas.

As an application, the Helmholtz relation turns [pressure](../../../../../pressure-split.md) data into an isothermal [entropy](../../../../../entropy-split.md) change. For an [ideal gas](../../../../../ideal-gas-split.md), $(\partial p/\partial T)_V=nR/V$, giving

$$
\boxed{\Delta S_{T}=\int_{V_1}^{V_2}\left(\frac{\partial p}{\partial T}\right)_VdV
=nR\ln\frac{V_2}{V_1}.}
$$

Combining the same relation with $dU=T\,dS-p\,dV$ yields $(\partial U/\partial V)_T=T(\partial p/\partial T)_V-p$, which vanishes for an [ideal gas](../../../../../ideal-gas-split.md) and reveals attractive-energy effects for a van der Waals gas. **[Thermodynamic potentials](../../../../../thermodynamic-potential-split.md) organize equilibrium constraints, while [Maxwell relations](../../../../../maxwell-relations.md) convert difficult [entropy](../../../../../entropy-split.md) [derivatives](../../../../../derivative.md) into measurable response [derivatives](../../../../../derivative.md).**

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
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
