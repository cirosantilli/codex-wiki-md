<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the same [atomic fractions](../../../../../atomic-fraction.md) and collision assumptions as in part(c). Let $A$ be the irradiated area. The number of atoms in the sheet is $N_t=ntA$, while the number of incident [neutrons](../../../../../neutron-split.md) is $\Phi A$, where $\Phi$ is the [neutron fluence](../../../../../neutron-fluence.md).

Counting one [primary knock-on atom](../../../../../primary-knock-on-atom.md) for each neutron that scatters and using $\nu=430$ displacements per recoil gives the first-collision estimate

$$
\begin{aligned}
d&=\frac{\nu\Phi A P_s}{ntA}\\
&=\frac{430(4\times10^{26})(0.0273697)}
{(8.6452\times10^{28})(10^{-3})}\\
&=54.45.
\end{aligned}
$$

Hence **the nominal damage is about $55$ [displacements per atom](../../../../../displacements-per-atom.md)** under the assumed composition. In the thin-sheet approximation the density and thickness cancel:

$$
\boxed{d\simeq\nu\Phi\bar\sigma_s
=430(4\times10^{26})(3.21\times10^{-28})=55.21.}
$$

The $1.4\%$ difference comes from using first-collision attenuation rather than the linear approximation. Treating repeated collisions after deflection would require angular and energy information not provided; this correction is already smaller than the precision warranted by the composition assumption.

There is also a counting convention in “other atoms”: $430$ counts secondary displacements, while including the displaced [primary knock-on atom](../../../../../primary-knock-on-atom.md) itself gives $\nu=431$. The corresponding first-collision result is $54.58$ rather than $54.45$ dpa, an increase of only $0.23\%$. Both conventions round to about $55$ dpa. The numerical estimate is explicitly conditional on assigning the stated displacement yield to each scattering event.

A value greater than one is physically possible. [Displacements per atom](../../../../../displacements-per-atom.md) counts displacement events relative to the initial atom inventory: atoms can be displaced repeatedly, and many [vacancies](../../../../../vacancy.md) and [self-interstitials](../../../../../self-interstitial.md) recombine. It does not mean $55$ surviving vacant sites per original lattice site, or that every atom has moved exactly $55$ times. This is a large nominal exposure for which evolving [dislocation loops](../../../../../dislocation-loop.md), cavities and [irradiation hardening](../../../../../irradiation-hardening.md) matter; the surviving [microstructure](../../../../../microstructure.md) additionally depends on [irradiation temperature](../../../../../irradiation-temperature.md), [displacement dose rate](../../../../../displacement-dose-rate.md), recombination and [defect sinks](../../../../../defect-sink.md).

## ↑ Ancestors (10)

1. [D](../d.md)
2. [2](../../2.md)
3. [Module NE3](../../../paper-ne3-split.md)
4. [2020](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
