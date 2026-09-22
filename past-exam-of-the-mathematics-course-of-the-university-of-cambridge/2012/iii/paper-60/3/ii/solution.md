<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $X$ be the [hydrogen mass fraction](../../../../../../hydrogen-mass-fraction.md), $f_g=\rho_g/\rho_{\rm tot}$ the gravitating gas fraction, and $\chi=n_{\rm tot}/n_H$ the total-particle-to-hydrogen ratio. The [optically thin gas cooling time](../../../../../../optically-thin-gas-cooling-time.md) and [free-fall time of a uniform sphere](../../../../../../free-fall-time-of-a-uniform-sphere.md) are

$$
t_{\rm cool}=\frac{(3/2)n_{\rm tot}k_BT}{n_H^2\Lambda}=\frac{3\chi k_BT}{2n_H\Lambda},\qquad t_{\rm ff}=\sqrt{\frac{3\pi Xf_g}{32Gm_pn_H}},
$$

where $\rho_{\rm tot}=m_pn_H/(Xf_g)$. Equating them gives the [cooling-to-free-fall equality curve](../../../../../../cooling-to-free-fall-equality-curve.md):

$$
\boxed{n_{H,{\rm crit}}(T)=\frac{32Gm_p}{3\pi Xf_g}\left(\frac{3\chi k_BT}{2\Lambda(T)}\right)^2.}
$$

At fixed composition, its shape is $n_{\rm crit}\propto T^2/\Lambda^2$. **Gas above this curve cools faster than it falls; gas below it cools more slowly.** Strong line cooling produces a deep low-density trough. In the high-temperature free-free regime, $\Lambda\propto T^{1/2}$ gives $n_{\rm crit}\propto T$.

<a id="3/ii/image-cooling-versus-free-fall-diagram-with-uniform-cloud-virial-mass-contours-and-illustrative-virial-densities"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-60-cooling-diagram.png)

**[Figure 3](#3/ii/image-cooling-versus-free-fall-diagram-with-uniform-cloud-virial-mass-contours-and-illustrative-virial-densities). Cooling versus free-fall diagram with uniform-cloud virial mass contours and illustrative virial densities**.

The displayed uniform self-gravitating-cloud example uses $f_g=1$, $X=0.76$, $\mu\simeq0.59$ and $\chi\simeq2.24$. Holding these ionized-gas factors fixed makes the diagram transparent, but near the atomic threshold their actual temperature dependence changes numerical normalizations. With these conventions the supplied cooling values imply $n_{\rm crit}(1.5\times10^4\,\mathrm K)\simeq9.6\times10^{-10}\,\mathrm{cm^{-3}}$ and $n_{\rm crit}(10^7\,\mathrm K)\simeq0.107\,\mathrm{cm^{-3}}$. For gas supported in a dark-matter-dominated [dark matter halo](../../../../../../dark-matter-halo.md), take $f_g<1$: at fixed $n_H$ the [free-fall time of a uniform sphere](../../../../../../free-fall-time-of-a-uniform-sphere.md) is shorter and the critical curve shifts upward by $1/f_g$.

To add [virial mass contours in a cooling diagram](../../../../../../virial-mass-contours-in-a-cooling-diagram.md), use the uniform self-gravitating sphere consistently. Its [Newtonian gravitational potential energy](../../../../../../newtonian-gravitational-potential-energy.md) is $-3GM^2/(5R)$ and its thermal [kinetic energy](../../../../../../kinetic-energy.md) is $(3/2)Mk_BT/(\mu m_p)$. The [virial theorem](../../../../../../virial-theorem.md) gives $k_BT_{\rm vir}=\mu m_pGM/(5R)$, while $M=(4\pi/3)R^3\rho_{\rm tot}$. Eliminating $R$ gives

$$
\boxed{n_H=\frac{375Xf_gk_B^3T_{\rm vir}^3}{4\pi G^3\mu^3m_p^4M^2}.}
$$

Thus constant total gravitating mass gives slope three in the logarithmic density-temperature plane, with larger mass contours lying at smaller density. A different density profile changes the structural coefficient; the customary halo temperature scale $k_BT_{\rm vir}=\mu m_pGM/(2R)$ shifts the mass contours but preserves their slopes. The horizontal illustrative formation-density lines are $n_{H,{\rm vir}}\simeq\Delta_v(2\times10^{-7})(1+z)^3\,\mathrm{cm^{-3}}$, using $\Delta_v=18\pi^2$. They show why increasing formation [cosmological redshift](../../../../../../cosmological-redshift.md) helps gas reach the rapid-cooling region.

At the low-mass end, a [dark matter halo](../../../../../../dark-matter-halo.md)'s [virial temperature](../../../../../../virial-temperature.md) may not reach the atomic threshold. The [atomic and molecular cooling thresholds for galaxy formation](../../../../../../atomic-and-molecular-cooling-thresholds-for-galaxy-formation.md) therefore favor an atomic-cooling mass of order $10^8M_\odot$ at early formation epochs, with its precise value varying as approximately $(1+z)^{-3/2}$. Smaller primordial systems require molecules; [photoheating](../../../../../../photoionization-heating.md) and [stellar feedback](../../../../../../stellar-feedback.md) further suppress their luminous output.

At the high-mass end, the [virial temperature](../../../../../../virial-temperature.md) at a fixed assembly density scales as $M^{2/3}$. Beyond the line-cooling interval the gas becomes increasingly hot, while [thermal bremsstrahlung](../../../../../../thermal-bremsstrahlung.md) improves only as $T^{1/2}$. Hence at fixed assembly density $t_{\rm cool}/t_{\rm ff}\propto T^{1/2}\propto M^{1/3}$ in that regime. Large systems can remain pressure-supported hot atmospheres for many dynamical times, instead of promptly fragmenting into one stellar object. This is the [upper galaxy mass from gas cooling](../../../../../../upper-galaxy-mass-from-gas-cooling.md): it associates efficient condensation with roughly galactic, rather than group or cluster, masses and motivates the broad $10^8$–$10^{12}M_\odot$ interval.

**The diagram gives characteristic cooling scales, not exact universal mass bounds.** Density profiles, gas fraction, enrichment and formation epoch move the boundaries; the two supplied values alone do not determine a complete numerical cutoff. Some gas can cool in dense cores of larger [dark-matter haloes](../../../../../../dark-matter-halo.md), early smaller progenitors can form stars before merging, and subsequent [galaxy mergers](../../../../../../galaxy-merger.md) can assemble more massive galaxies. Long-lived hot atmospheres also require heating to prevent excessive late-time cooling. These qualifications explain why the [cooling criterion for galaxy formation](../../../../../../cooling-criterion-for-galaxy-formation.md) is useful without equating each dark [dark matter halo](../../../../../../dark-matter-halo.md) to one galaxy.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
