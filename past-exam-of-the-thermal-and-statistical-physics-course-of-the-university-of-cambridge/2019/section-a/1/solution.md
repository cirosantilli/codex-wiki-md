<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Gibbs-Duhem equation](../../../../gibbs-duhem-equation.md) for a homogeneous, extensive, single-component [thermodynamic phase](../../../../thermodynamic-phase.md):

$$
S\,dT-V\,dp+N\,d\mu=0.
$$

At fixed [temperature](../../../../temperature-split.md), this becomes $dp=n\,d\mu$, with [number density](../../../../number-density.md) $n=N/V$. Separately, at fixed [particle number](../../../../particle-number.md),

$$
\left(\frac{\partial n}{\partial p}\right)_{T,N}
=-\frac{N}{V^2}\left(\frac{\partial V}{\partial p}\right)_{T,N}
=n\kappa_T.
$$

The [chain rule](../../../../chain-rule.md) along the same [isothermal process](../../../../isothermal-process.md) in the [equation of state](../../../../equation-of-state.md) now gives

$$
\left(\frac{\partial n}{\partial\mu}\right)_T
=\left(\frac{\partial n}{\partial p}\right)_T
\left(\frac{\partial p}{\partial\mu}\right)_T
=n\kappa_T\,n.
$$

Consequently

$$
\boxed{\kappa_T=\frac1{n^2}\left(\frac{\partial n}{\partial\mu}\right)_T.}
$$

This is [isothermal compressibility from chemical-potential response](../../../../isothermal-compressibility-from-chemical-potential-response.md). Since [chemical potential](../../../../chemical-potential-split.md) has units of [energy](../../../../energy-split.md) per particle, the right-hand side has units of [volume](../../../../volume-thermodynamics.md) per [energy](../../../../energy-split.md), or $\mathrm{Pa^{-1}}$, as required. The derivation assumes a smooth bulk [equation of state](../../../../equation-of-state.md); changing the fractions of coexisting [thermodynamic phases](../../../../thermodynamic-phase.md) at fixed [pressure](../../../../pressure-split.md) needs separate treatment.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
