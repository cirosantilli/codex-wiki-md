<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Use the [Feynman parameters](../../../../feynman-parameter.md) and $J_3$ defined in [Solution](../iv/solution.md). With $A=4C$, the finite term just found is $-C\Delta J_3$. Combining it with the remaining $g_{\mu\nu}$ coefficient gives

$$
C[-\Delta+m^2-s/2+sxy]J_3
=-\frac{sC}{2}(1-4xy)J_3.
$$

The other coefficient is $(B-4Cxy)J_3$. Thus, writing $\mathscr I_{\mu\nu}$ for the [Feynman integral](../../../../feynman-integral.md) without the overall prefactor,

$$
\mathscr I_{\mu\nu}=2\int_{\mathcal T}dx\,dy\,J_3(\Delta)
\left[-\frac{sC}{2}(1-4xy)g_{\mu\nu}+(B-4Cxy)p_{2,\mu}p_{1,\nu}\right].
$$

For $T_{\mu\nu}=\frac s2g_{\mu\nu}-p_{2,\mu}p_{1,\nu}$, the two coefficients must have the corresponding ratio. The mismatch is simply $(B-C)J_3$, independent of $xy$. Therefore the required relation is

$$
\boxed{B=C,}
$$

which is satisfied. In the primitive normalization the result is

$$
\mathscr I_{\mu\nu}=\frac{i}{16\pi^2}\int_0^1dx\int_0^{1-x}dy\,
\frac{1-4xy}{m^2-sxy-i0}\,T_{\mu\nu},
$$

and the full [top quark](../../../../top-quark.md) [scattering amplitude](../../../../scattering-amplitude.md), in our stated $S$ convention, is

$$
\boxed{\mathcal M=-\frac{N_cye^2Q^2m}{2\pi^2}\,
\epsilon_1^\mu\epsilon_2^\nu T_{\mu\nu}
\int_0^1dx\int_0^{1-x}dy\,\frac{1-4xy}{m^2-sxy-i0}.}
$$

Indeed $p_1^\mu T_{\mu\nu}=p_2^\nu T_{\mu\nu}=0$: replacing either [polarization vector](../../../../polarization-vector.md) by its [photon](../../../../photon.md) [momentum](../../../../momentum-split.md) makes the [scattering amplitude](../../../../scattering-amplitude.md) vanish. This is the [Ward identity](../../../../ward-identity.md), expressing electromagnetic [gauge invariance](../../../../gauge-invariance.md). The result also is symmetric under exchange of the two [photons](../../../../photon.md). The finite term in [Solution](../iv/solution.md) is essential for this [Ward identity](../../../../ward-identity.md).

As an independent low-[energy](../../../../energy-split.md) check, for $s/m^2\to0$ the [Feynman parameter](../../../../feynman-parameter.md) integral is

$$
\frac1{m^2}\int_{\mathcal T}(1-4xy)\,dx\,dy+O(s/m^4)
=\frac1{3m^2}+O(s/m^4).
$$

The coefficient is consequently $-N_cye^2Q^2/(6\pi^2m)$ at leading order. It has the inverse-[mass](../../../../mass.md) dimension required for an effective $hF_{\mu\nu}F^{\mu\nu}$ coupling. If $y=m/v$, this coefficient stays finite in the large-$m$ limit at fixed $v$; that limit increases the [Yukawa coupling](../../../../yukawa-interaction.md), so it is not a fixed-coupling [heavy-field decoupling](../../../../heavy-field-decoupling.md) limit.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the advanced quantum field theory course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory course of the University of Oxford](../../../../advanced-quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
