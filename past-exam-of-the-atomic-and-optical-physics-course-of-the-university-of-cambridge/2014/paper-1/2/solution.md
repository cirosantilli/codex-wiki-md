<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Set the ground-state [energy](../../../../energy-split.md) to zero. Bose-Einstein occupation of an excited level is $[e^{(\epsilon-\mu)/(k_BT)}-1]^{-1}$, with $\mu\le0$. As particles are added, $\mu$ approaches zero and the excited-state population saturates. Separating the ground state from the density-of-states integral therefore gives

$$
\boxed{N_c(T)=\int_0^\infty\frac{g(\epsilon)\,d\epsilon}{e^{\epsilon/(k_BT)}-1},
\qquad\frac{N_0}{N}=1-\frac1\eta.}
$$

The excited-state integral must actually converge: $g\to0$ alone is not a sufficient condition in complete generality. A [power](../../../../power.md) law $g\propto\epsilon^s$ with $s>0$ suffices at low [energy](../../../../energy-split.md), as in the stated three-dimensional box.

Let $\mathcal C=Vm^{3/2}/(\sqrt2\pi^2\hbar^3)$ denote the density-of-states prefactor, not a [heat capacity](../../../../heat-capacity.md). Substitution $x=\epsilon/(k_BT)$ gives

$$
N_c=\mathcal C(k_BT)^{3/2}\Gamma(3/2)\zeta(3/2)
=\boxed{\zeta(3/2)\frac V{\lambda^3}}.
$$

The condensate has zero [energy](../../../../energy-split.md) on this reference, so a further factor of $\epsilon$ in the integral gives

$$
E=\mathcal C(k_BT)^{5/2}\Gamma(5/2)\zeta(5/2),
\qquad
\boxed{\frac EN=\frac32\frac{N_c}{N}
\frac{\zeta(5/2)}{\zeta(3/2)}k_BT.}
$$

Relative to the classical value, the ratio is $\zeta(5/2)/[\eta\zeta(3/2)]\simeq0.5134/\eta<0.5134$. Macroscopic occupation of the zero-energy state and the Bose distribution both lower the average [energy](../../../../energy-split.md).

At fixed volume the condensed gas has $E\propto T^{5/2}$. Unbiased random loss keeps average $E/N$ constant, hence

$$
\boxed{T\propto N^{2/5}.}
$$

Removing a condensate atom removes essentially no [energy](../../../../energy-split.md) and by itself leaves the excited cloud's [temperature](../../../../temperature-split.md) unchanged. Removing an excited atom removes its [energy](../../../../energy-split.md); during re-equilibration, some zero-energy condensate atoms join the excited population and share the remaining [energy](../../../../energy-split.md), lowering [temperature](../../../../temperature-split.md). Averaging over unbiased loss gives the stated constant [energy](../../../../energy-split.md) per particle, even though each individual type of loss need not preserve it separately.

Using $m\simeq87u$ and the supplied volume,

$$
\lambda_i\simeq0.837\,\mathrm{\mu m},\quad
N_c(T_i)\simeq1.78\times10^5,\quad
\boxed{\eta_i\simeq1.68.}
$$

There is only one occupied internal [spin](../../../../spin.md) state, so no factor $2F+1$ belongs in the [density of states](../../../../density-of-states.md). During loss, $\eta\propto N/T^{3/2}\propto N^{2/5}$, hence $\eta/\eta_i=T/T_i$. Condensation disappears at $\eta_f=1$:

$$
\boxed{T_f=\frac{T_i}{\eta_i}\simeq29.7\,\mathrm{nK}.}
$$

As a consistency check, $N_f=N_i\eta_i^{-5/2}\simeq8.15\times10^4$ agrees with $N_c(T_f)$.

Both this process and [evaporative cooling of atoms](../../../../evaporative-cooling-atomic-physics.md) require particle loss and re-equilibration. Ordinary evaporation preferentially removes energetic atoms, reducing $E/N$, and can cool an uncondensed classical gas. Here loss is [energy](../../../../energy-split.md) independent, $E/N$ stays constant, and cooling relies on the condensed gas's unusual [equation of state](../../../../equation-of-state.md); random loss of a classical [ideal gas](../../../../ideal-gas-split.md) would leave its [temperature](../../../../temperature-split.md) unchanged. Exact noninteraction would prevent collisional rethermalization: the imposed equilibrium assumption can be understood as weak thermalizing interactions whose equation-of-state corrections are neglected.

<a id="2/image-temperature-and-condensate-fraction-during-unbiased-loss-ending-at-the-condensation-threshold"></a>
![](../../../../past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2014/paper-1-aop-random-loss.png)

**[Figure 2](#2/image-temperature-and-condensate-fraction-during-unbiased-loss-ending-at-the-condensation-threshold). Temperature and condensate fraction during unbiased loss, ending at the condensation threshold**.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the atomic and Optical Physics course of the University of Cambridge](../../../split.md)
5. [Atomic and Optical Physics course of the University of Cambridge](../../../../atomic-and-optical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
