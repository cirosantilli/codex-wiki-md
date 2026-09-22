<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume a homogeneous Fe–Cr–Ni [alloy](../../../../../alloy.md), normal incidence, independent scattering events and the stated effective [scattering cross-sections](../../../../../scattering-cross-section.md). Neglect absorption, other constituents and changes in neutron energy within the thin sheet. The [atomic fractions](../../../../../atomic-fraction.md) are not supplied; **take $x_{\rm Fe}=0.70$, $x_{\rm Cr}=0.20$, $x_{\rm Ni}=0.10$ as an explicit representative assumption**, not a composition measured or specified in the paper.

The conventional cell of a [face-centered cubic lattice](../../../../../face-centered-cubic-lattice.md) contains

$$
8\left(\frac18\right)+6\left(\frac12\right)=4
$$

atoms. The [number density](../../../../../number-density.md) is therefore

$$
n=\frac4{a^3}=\frac4{(0.359\times10^{-9})^3}
=8.6452\times10^{28}\ \mathrm{m^{-3}}.
$$

For a mixture, the scattering probability per unit path length is $\Sigma_s=\sum_j n_j\sigma_j=n\bar\sigma_s$, where

$$
\begin{aligned}
\bar\sigma_s&=\sum_jx_j\sigma_j\\
&=[0.70(3.2)+0.20(2.8)+0.10(4.1)]\times10^{-28}\\
&=3.21\times10^{-28}\ \mathrm{m^2}.
\end{aligned}
$$

Thus $\Sigma_s=27.751\ \mathrm{m^{-1}}$. For thickness $t=10^{-3}\,\mathrm m$, the unscattered fraction $U$ satisfies $dU/dz=-\Sigma_sU$ with $U(0)=1$. The fraction undergoing at least one [neutron scattering](../../../../../neutron-scattering.md) event is

$$
\boxed{P_s=1-e^{-\Sigma_st}=1-e^{-0.027751}=0.027370\simeq2.74\%.}
$$

The thin-sheet approximation gives $P_s\simeq\Sigma_st=2.78\%$, consistent to the accuracy of the assumed composition. A simple iron-dominated estimate $\bar\sigma_s\simeq3.2$ [barns](../../../../../barn-unit.md) gives essentially the same **about $3\%$ scattered** conclusion.

For any other assumed composition, use the displayed weighted formula; mass fractions must first be converted to [atomic fractions](../../../../../atomic-fraction.md). Since the supplied elemental cross-sections span $2.8$–$4.1$ [barns](../../../../../barn-unit.md), any mixture of these three elements at the stated [number density](../../../../../number-density.md) gives approximately $2.39$–$3.48\%$. This is a bound within the idealized mixture model, not a claim that every such composition is stable [austenite](../../../../../austenite.md).

## ↑ Ancestors (10)

1. [C](../c.md)
2. [2](../../2.md)
3. [Module NE3](../../../paper-ne3-split.md)
4. [2020](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
