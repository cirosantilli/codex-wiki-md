<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [solar corona](../../../../../solar-corona.md) is a hot, dilute [plasma](../../../../../plasma-physics.md) in which [collisional ionization](../../../../../collisional-ionization.md) mainly proceeds by direct [Electron](../../../../../electron.md) impact and by [excitation-autoionization](../../../../../excitation-autoionization.md). The principal inverse ion-changing processes are [radiative recombination](../../../../../radiative-recombination.md) and [dielectronic recombination](../../../../../dielectronic-recombination.md). [Three-body recombination](../../../../../three-body-recombination.md) is negligible at ordinary coronal densities. Photoionization, stimulated recombination and charge exchange are normally secondary in this fully ionized, collision-dominated regime, although they should be reconsidered near irradiated or neutral interfaces.

For [collisional ionization equilibrium](../../../../../collisional-ionization-equilibrium.md), the adjacent [ion](../../../../../ion.md) stages satisfy

$$
N_eN_qC_q(T_e)=N_eN_{q+1}\alpha_{q+1}(T_e),
$$

together with conservation of the element's total abundance. Thus the low-density [ion](../../../../../ion.md) fraction depends primarily on $T_e$. This fixes the amount of Si X available for line emission, but not the populations of its excited levels: a [coronal approximation](../../../../../coronal-approximation.md) does not impose a Boltzmann level distribution.

Within an [ion](../../../../../ion.md), [Electrons](../../../../../electron.md) collisionally excite, de-excite and redistribute levels. Their [collision rate coefficient for an atomic transition](../../../../../collision-rate-coefficient-for-an-atomic-transition.md) is

$$
q_{ij}(T_e)=\int_0^\infty\sigma_{ij}(v)v f_{T_e}(v)\,dv.
$$

The rate per [ion](../../../../../ion.md) is $N_eq_{ij}$. Maxwellian detailed balance gives, for $E_j>E_i$,

$$
q_{ji}=\frac{g_i}{g_j}e^{(E_j-E_i)/kT_e}q_{ij}.
$$

Strong allowed transitions undergo rapid [spontaneous emission](../../../../../spontaneous-emission.md); forbidden magnetic-dipole and electric-quadrupole transitions give much smaller decay rates and can leave a [metastable atomic level](../../../../../metastable-atomic-level.md) appreciably populated. [Radiative cascades](../../../../../radiative-cascade.md) feed levels from higher states. Absorption and stimulated emission add rates proportional to the local radiation field through the [Einstein coefficients](../../../../../einstein-coefficients.md) when significant. Proton collisions can also mix closely separated levels separated by [fine structure](../../../../../fine-structure.md) and should be included when their rates matter.

Write $f_i=N_i/N(\mathrm{Si\ X})$. A stationary [collisional-radiative model](../../../../../collisional-radiative-model.md) solves

$$
\boxed{\sum_{j\ne i}f_jP_{ji}-f_i\sum_{j\ne i}P_{ij}=0,
\qquad\sum_i f_i=1,}
$$

where, in the simplest electron-plus-radiative model, $P_{ij}=N_eq_{ij}+A_{ij}$ with $A_{ij}=0$ for an upward transition. Add proton and radiation rates when appropriate. Include enough levels and radiative branches to capture population feeding. The thermal collision data, radiative probabilities and wavelengths then determine each line's [optically thin atomic line intensity](../../../../../optically-thin-atomic-line-intensity.md):

$$
\boxed{I_{ul}=\frac{h\nu_{ul}}{4\pi}\int N(\mathrm{Si\ X})f_u(N_e,T_e)A_{ul}\,ds.}
$$

The factor $4\pi$ distributes isotropic emission over [solid angle](../../../../../solid-angle.md). [photon](../../../../../photon.md) intensities omit $h\nu$. A practical source of the necessary atomic rates and population calculations is the [CHIANTI reference guide](https://www.chiantidatabase.org/cug.pdf).

Label the two ground-configuration levels $1,2$ and the two indicated excited levels $3,4$:

$$
\begin{aligned}
1&:2s^22p\,{}^2P_{1/2},&2&:2s^22p\,{}^2P_{3/2},\\
3&:2s2p^2\,{}^2D_{3/2},&4&:2s2p^2\,{}^2D_{5/2}.
\end{aligned}
$$

The common $1s^2$ core is omitted. Si X is silicon with nine [Electrons](../../../../../electron.md) removed, hence five bound [Electrons](../../../../../electron.md); the left superscript $2$ on $P$ or $D$ is the spin multiplicity, not another electron-occupancy exponent.

The observed lines correspond to decays $3\to1$ and $4\to2$. For approximately uniform [plasma](../../../../../plasma-physics.md) at the indicated $T_e\simeq1.3\times10^6\,\mathrm K$, form the theoretical energy-intensity ratio

$$
\boxed{R(N_e)=\frac{I_{356}}{I_{347}}
=\frac{\nu_{42}A_{42}f_4(N_e,T_e)}{\nu_{31}A_{31}f_3(N_e,T_e)}.}
$$

The common abundance, Si X fraction and path length cancel, leaving a ratio governed by level populations. The frequency factor is $\nu_{42}/\nu_{31}=347/356$ for the rounded wavelengths. With observed [photon](../../../../../photon.md) counts, first apply the detector calibration and use the corresponding photon-ratio convention.

The [electron-density diagnostic from metastable populations](../../../../../electron-density-diagnostic-from-metastable-populations.md) can be seen in a reduced rate model. The upper ground level $2$ has only a weak radiative decay to $1$. Ignoring higher-level feeding for this explanation, their balance gives

$$
r:=\frac{N_2}{N_1}=\frac{N_eq_{12}}{A_{21}+N_eq_{21}}.
$$

At low density $r\simeq N_eq_{12}/A_{21}$; above the [critical density of an atomic transition](../../../../../critical-density-of-an-atomic-transition.md) $A_{21}/q_{21}$ it approaches $q_{12}/q_{21}=(g_2/g_1)e^{-\Delta E_{21}/kT_e}$, approximately two when the gap due to [fine structure](../../../../../fine-structure.md) is small compared with $kT_e$. This saturation can occur while the strong upper-level transitions still remain radiatively dominated.

Let $A_3,A_4$ be the total radiative loss rates of levels $3,4$, and $b_{31}=A_{31}/A_3$, $b_{42}=A_{42}/A_4$ their line branching fractions. In that upper-level low-density regime,

$$
N_3\simeq\frac{N_e(N_1q_{13}+N_2q_{23})}{A_3},\qquad
N_4\simeq\frac{N_e(N_1q_{14}+N_2q_{24})}{A_4}.
$$

Thus

$$
R\simeq K\frac{q_{14}+r q_{24}}{q_{13}+r q_{23}},\qquad
K=\frac{\nu_{42}b_{42}}{\nu_{31}b_{31}}.
$$

The two lines receive different relative feeding from the two ground levels, so their ratio changes as collisions populate the metastable level. More explicitly,

$$
\frac{dR}{dr}=K\frac{q_{24}q_{13}-q_{14}q_{23}}{(q_{13}+r q_{23})^2}.
$$

Different, nonproportional feeding coefficients give a usable density-sensitive interval. With $s=R/K$, this reduced model even permits explicit inversion:

$$
\boxed{r=\frac{s q_{13}-q_{14}}{q_{24}-s q_{23}},\qquad
N_e=\frac{A_{21}r}{q_{12}-r q_{21}}.}
$$

Physical solutions require positive density and a ratio within the allowed calibration range. The actual Si X calibration should use the full multilevel population system, not discard cross-excitation, cascades or all competing branches simply to use this illustrative formula.

Operationally, evaluate the model ratio at the known [temperature](../../../../../temperature.md) over a density grid and match the calibrated observed ratio to it, propagating line-flux and atomic-data uncertainties. No observed ratio or numerical atomic rate set is supplied here, so the result is this inference procedure rather than a numerical density. At low- or high-density saturation, the ratio constrains density poorly. Deconvolve blends or sum every unresolved transition in the theoretical feature; for example, the neighboring $^2D_{3/2}\to{}^2P_{3/2}$ branch can contribute near the 356-Angstrom feature when unresolved. Atomic line identifications and that nearby branch are tabulated in [Del Zanna's coronal-spectroscopy thesis](https://www.damtp.cam.ac.uk/user/astro/gd232/research/thesis/gdz_phd_thesis.pdf).

For a nonuniform sightline, the ratio is instead

$$
R_{\rm obs}=\frac{\int j_{347}(s)R(N_e(s),T_e(s))\,ds}{\int j_{347}(s)\,ds}.
$$

A single-density inversion gives an [emission-weighted effective density from a line ratio](../../../../../emission-weighted-effective-density-from-a-line-ratio.md), generally not the volume-average [electron number density](../../../../../electron-number-density.md). **The density estimate is meaningful within its [temperature](../../../../../temperature.md), optical-depth, line-blending and spatial-uniformity assumptions.** This is the precise interpretation of an average density obtained from the observed pair.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
