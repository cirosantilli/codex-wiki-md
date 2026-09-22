<h1 id="section-b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Canonical [probabilities](../../../../probability.md).** A [canonical ensemble](../../../../canonical-ensemble-split.md) describes a system of fixed [particle number](../../../../particle-number.md) and fixed external parameters such as [volume](../../../../volume-thermodynamics.md), weakly coupled to a much larger [thermal reservoir](../../../../heat-bath.md). They exchange [energy](../../../../energy-split.md) and reach [thermal equilibrium](../../../../thermal-equilibrium-split.md), while the reservoir's [temperature](../../../../temperature-split.md) stays effectively constant. The interaction [energy](../../../../energy-split.md) is negligible in the state counting. The combined isolated system is described by equal [probabilities](../../../../probability.md) for its accessible [microstates](../../../../microstate.md).

If its total [energy](../../../../energy-split.md) is $E_{\mathrm{tot}}$, the [probability](../../../../probability.md) of a particular system [microstate](../../../../microstate.md) $i$ is proportional to the reservoir multiplicity at $E_{\mathrm{tot}}-E_i$. Writing that multiplicity as $e^{S_R/k_B}$, expand its [entropy](../../../../entropy-split.md):

$$
S_R(E_{\mathrm{tot}}-E_i)
=S_R(E_{\mathrm{tot}})-\left(\frac{\partial S_R}{\partial E_R}\right)E_i+\cdots
=S_R(E_{\mathrm{tot}})-\frac{E_i}{T}+\cdots.
$$

The large-reservoir limit suppresses the higher terms. Normalization therefore gives

$$
\boxed{P_i=\frac{e^{-\beta E_i}}{Z},\qquad
Z=\sum_j e^{-\beta E_j},\qquad\beta=\frac1{k_BT}.}
$$

The sum counts individual [microstates](../../../../microstate.md); when grouping them by [energy](../../../../energy-split.md), their [state degeneracies](../../../../state-degeneracy.md) must be included. This $Z$ is the [canonical partition function](../../../../canonical-partition-function.md).

**Classical orientational [heat capacity](../../../../heat-capacity.md).** Hold the [magnetic field](../../../../magnetic-field-split.md) fixed. Orientations of the [magnetic dipole moment](../../../../magnetic-dipole-moment.md) have the [solid angle](../../../../solid-angle.md) [measure](../../../../measure-split.md) $d\Omega=\sin\theta\,d\theta\,d\varphi$. With $x=\beta mB$, the angular [partition function](../../../../canonical-partition-function.md) is

$$
Z_{\mathrm{ang}}=\int e^{x\cos\theta}d\Omega
=2\pi\int_{-1}^{1}e^{xu}du
=4\pi\frac{\sinh x}{x}.
$$

Choosing a normalized angular [measure](../../../../measure-split.md) would remove $4\pi$, with no effect on the [energy](../../../../energy-split.md) [derivatives](../../../../derivative.md). Differentiating at fixed $B$,

$$
U=-\frac{\partial\ln Z_{\mathrm{ang}}}{\partial\beta}
=-mB\left(\coth x-\frac1x\right)
=-mB\coth x+k_BT.
$$

The angular average $\langle\cos\theta\rangle=\coth x-1/x$ is the [Langevin function](../../../../langevin-function.md). Since $dx/dT=-x/T$,

$$
\boxed{C_B=\left(\frac{\partial U}{\partial T}\right)_B
=k_B\left[1-\left(\frac{x}{\sinh x}\right)^2\right].}
$$

This is the [heat capacity of a classical magnetic dipole](../../../../heat-capacity-of-a-classical-magnetic-dipole.md), in $\mathrm{J\,K^{-1}}$ for one [magnetic moment](../../../../magnetic-dipole-moment.md). The word specific here refers to that single moment; $N$ independent [magnetic moments](../../../../magnetic-dipole-moment.md) have $N$ times this [heat capacity](../../../../heat-capacity.md). At $B=0$ the [energy](../../../../energy-split.md) is independent of orientation and $C_B=0$, obtained by the continuous $x\to0$ limit. At fixed nonzero $B$, the classical low-temperature limit instead gives $C_B\to k_B$.

**Equipartition and its proof.** The [equipartition theorem](../../../../equipartition-theorem.md) states that an independent quadratic term $a q^2/2$ in a classical [Hamiltonian](../../../../hamiltonian.md), with $a>0$, contributes $k_BT/2$ to its mean [energy](../../../../energy-split.md). One needs a canonical [measure](../../../../measure-split.md) that factors as $dq$ times the [measure](../../../../measure-split.md) of the remaining variables, convergence of the [integrals](../../../../integral-split.md), and vanishing boundary terms. The coordinate must not be restricted by a thermally important hard boundary or a coupled [constraint](../../../../constraint-mechanics.md).

For $H=a q^2/2+H_0$, [integration by parts](../../../../integration-by-parts.md) gives

$$
0=\int_{-\infty}^{\infty}\frac\partial{\partial q}
\left(qe^{-\beta H}\right)dq
=\int_{-\infty}^{\infty}\left(1-\beta q\frac{\partial H}{\partial q}\right)e^{-\beta H}dq.
$$

Integrate over all other variables and divide by $Z$. It follows that

$$
\left\langle q\frac{\partial H}{\partial q}\right\rangle=k_BT,
\qquad
\boxed{\left\langle\frac{a q^2}{2}\right\rangle=\frac12k_BT.}
$$

The same reasoning applies to quadratic momenta among the [canonical variables](../../../../canonical-variables.md). It is the number of quadratic [energy](../../../../energy-split.md) contributions that is counted, not an unrestricted count of coordinate labels.

**Two soft orientational directions.** When $x\gg1$, the moment is concentrated near alignment. Introduce local [Cartesian coordinates](../../../../cartesian-coordinate-system.md) in the [tangent plane](../../../../tangent-plane.md) $q_1=\theta\cos\varphi$ and $q_2=\theta\sin\varphi$. To leading order,

$$
E=-mB+\frac{mB}{2}(q_1^2+q_2^2)+O(mB\theta^4),
\qquad d\Omega\simeq dq_1dq_2.
$$

The two quadratic terms each contribute $k_BT/2$, so

$$
\boxed{U=-mB+k_BT+o(T),\qquad C_B\longrightarrow k_B.}
$$

This agrees with the exact angular calculation. Treating $\theta$ alone as one Cartesian quadratic variable would miss the $\sin\theta$ [measure](../../../../measure-split.md) and the second tangent direction. There are no extra rotational kinetic terms in the stipulated [Hamiltonian](../../../../hamiltonian.md); adding such terms would be a different model.

**Quantum [spin](../../../../spin.md) one.** The [spin](../../../../spin.md) projections are $m_s=-1,0,1$, with $S_z=\hbar m_s$. Put $\Delta=\hbar|\gamma|B>0$, where $\gamma$ is the [gyromagnetic ratio](../../../../gyromagnetic-ratio.md). The three [energies](../../../../energy-split.md) are $-\Delta,0,+\Delta$, irrespective of the sign of $\gamma$. Relative to the [ground state](../../../../ground-state.md) they are $0,\Delta,2\Delta$. Thus, with $q=e^{-\beta\Delta}$,

$$
Z=e^{\beta\Delta}(1+q+q^2),\qquad
U=-\Delta+\Delta\frac{q+2q^2}{1+q+q^2}.
$$

Differentiation, or the [canonical energy fluctuation](../../../../canonical-energy-fluctuation.md) identity $C_B=k_B\beta^2\operatorname{Var}(E)$, gives

$$
C_B=k_B(\beta\Delta)^2
\frac{q(1+4q+q^2)}{(1+q+q^2)^2}.
$$

In the requested limit,

$$
\boxed{C_B\sim k_B\left(\frac{\Delta}{k_BT}\right)^2e^{-\Delta/(k_BT)},
\qquad\Delta=\hbar|\gamma|B.}
$$

This [spin-1 paramagnet](../../../../spin-1-paramagnet.md) has a nondegenerate [ground state](../../../../ground-state.md) and a finite [spectral gap](../../../../spectral-gap.md). Excitations are exponentially rare, so its [heat capacity](../../../../heat-capacity.md) tends to zero. Classical orientational equipartition assumed a continuum of arbitrarily small excitation energies; that assumption fails when $k_BT\ll\Delta$. This is a change in the accessible state spectrum, not a violation of the [equipartition theorem](../../../../equipartition-theorem.md) within its classical domain.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Section B](../../section-b.md)
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
