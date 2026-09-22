<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The principal feature is the abundance of planets with radii of roughly one to a few [Earth](../../../../earth.md) radii compared with large [gas giants](../../../../gas-giant.md) within the stated short-period sample. The smallest few plotted bins are of broadly similar height, followed by a substantial decline at larger sizes. Thus the figure supports **a high occurrence of small planets relative to giants**, rather than an indefinitely steep rise toward arbitrarily small sizes. The horizontal scale is logarithmic: one should compare counts in the displayed bins with their widths in $\ln R_p$, not mistake a bin count for a density per unit linear [radius](../../../../radius.md).

The vertical axis is an average number of planets per target [star](../../../../star.md). This [exoplanet occurrence rate](../../../../exoplanet-occurrence-rate.md) need not equal the fraction of stars hosting a planet, because one star can host several. The restriction to periods below $85$ days also matters: the figure is not a census of distant [gas giants](../../../../gas-giant.md) or of every planet in a system. Neither the detailed reduction procedure nor the raw detection counts are specified in the caption, so they cannot be reconstructed uniquely from the histogram.

Selection effects actually make the small-planet population harder to see. A full, undiluted [exoplanet transit depth](../../../../exoplanet-transit-depth.md) is approximately $(R_p/R_\star)^2$. For independent photometric errors of fractional size $\sigma_f$ per sample, an idealized detection [signal-to-noise ratio](../../../../signal-to-noise-ratio.md) is

$$
\mathrm{SNR}\simeq\frac{(R_p/R_\star)^2}{\sigma_f}\sqrt{N_{\rm in}},
$$

where $N_{\rm in}$ counts in-transit samples. At fixed [star](../../../../star.md) and [orbital period](../../../../orbital-period.md), halving planet [radius](../../../../radius.md) reduces this amplitude by four. Fainter hosts, correlated stellar noise, gaps and transit vetting reduce [transit survey completeness](../../../../transit-survey-completeness.md) further. [Geometric transit probability](../../../../geometric-transit-probability.md) also falls with orbital distance, $p_{\rm tr}\simeq R_\star/a\propto P^{-2/3}$ for fixed stellar [mass](../../../../mass.md). For a fixed observing baseline and cadence, the small-planet circular duration law gives $N_{\rm in}\propto P^{-2/3}$ and approximately $\mathrm{SNR}\propto R_p^2P^{-1/3}$.

Recovering an intrinsic [exoplanet occurrence rate](../../../../exoplanet-occurrence-rate.md) therefore requires correcting for geometric alignments, incomplete recovery and false positives. An illustrative estimator for a radius-period bin is

$$
f_{\mathcal B}\simeq\frac1{N_\star}\sum_{j\in\mathcal B}
\frac{w_j}{p_{{\rm tr},j}C_j},
$$

where $C_j$ is the recovery probability over the relevant target sample and $w_j$ accounts for candidate reliability. Real analyses must average these probabilities over heterogeneous targets and measurement uncertainty; the formula indicates the required weights, not a reconstruction of the unpublished inputs to this figure. A primary [Kepler space telescope](../../../../kepler-space-telescope.md) analysis explicitly models both false positives and incomplete detection to infer occurrence.[Sections V–VI: detection model and planet occurrence; Figure 7 distinguishes average number per star from hosting fraction](../../../../the-false-positive-rate-of-kepler-and-the-occurrence-of-planets-by-francois-fressin-and-others.md)

Thus the apparent preference for small planets cannot be explained by their being photometrically easier to detect. Small transits are harder. A plateau in occurrence below about twice Earth's size was independently reported using synthetic-transit injection and recovery, though that study used a different $5$–$50$-day selection and is not identified here as the source of the exam's plot.[Abstract: injection/recovery completeness, rise from large planets to about two Earth radii, plateau toward one Earth radius, and 5–50-day selection](../../../../a-plateau-in-the-planet-population-below-twice-the-size-of-earth-by-erik-a-petigura-and-others.md)

The natural physical framework is [core accretion](../../../../core-accretion.md) in a [protoplanetary disk](../../../../protoplanetary-disk.md). Most initial disk [mass](../../../../mass.md) is gas, principally [hydrogen](../../../../hydrogen.md) and [helium](../../../../helium.md); a much smaller fraction is solid material. [Protoplanetary dust coagulation](../../../../protoplanetary-dust-coagulation.md) first assembles aggregates through low-speed sticking. Settling and differential [drag](../../../../drag-physics.md) help concentrate solids, but bouncing, the [fragmentation barrier to dust growth](../../../../fragmentation-barrier-to-dust-growth.md) and [radial drift of solids in a gas disk](../../../../radial-drift-of-solids-in-a-gas-disk.md) prevent a simple assumption that every collision grows a body smoothly to planetary size. Concentration in [dust traps](../../../../dust-trap.md) or through [streaming instability](../../../../streaming-instability.md), followed by gravitational collapse of a dense solid population, provides routes to [planetesimals](../../../../planetesimal.md). Subsequent collisions must dissipate sufficient relative [energy](../../../../energy-split.md) to bind material rather than disrupt it.

Once sufficiently large [planetesimals](../../../../planetesimal.md) exist, [gravitational focusing](../../../../gravitational-focusing.md) enhances their accretion cross-sections:

$$
\sigma_{\rm coll}\simeq\pi R^2\left(1+\frac{v_{\rm esc}^2}{v_{\rm rel}^2}\right),
\qquad v_{\rm esc}^2\simeq\frac{2GM}{R}.
$$

When background random velocities remain small, larger bodies grow disproportionately fast in [runaway planetesimal growth](../../../../runaway-planetesimal-growth.md). As they become massive enough to stir the surrounding population, [oligarchic growth](../../../../oligarchic-growth.md) develops: several [planetary embryos](../../../../planetary-embryo.md) occupy neighboring [feeding zones](../../../../feeding-zone-of-a-planetary-embryo.md), while much of the remaining solid material resides in smaller [planetesimals](../../../../planetesimal.md). Heating the planetesimal random motions weakens [gravitational focusing](../../../../gravitational-focusing.md), and local depletion drives the embryos toward an [isolation mass](../../../../isolation-mass.md). Collisions among embryos can continue assembly after gas dispersal.

This solid-building pathway naturally produces many modest cores. Producing a large [gas giant](../../../../gas-giant.md) requires an additional, time-sensitive step: a sufficiently massive core must acquire and cool a gaseous envelope while disk gas remains available. Gas captured by a low-mass core releases [gravitational potential energy](../../../../gravitational-energy.md); the envelope's ability to radiate that energy governs its contraction and further accretion. A characteristic cooling estimate is

$$
t_{\rm cool}\sim\frac{|E_{\rm tot}|}{L_{\rm cool}},
$$

where $E_{\rm tot}$ includes the envelope’s gravitational and internal energies. This states an energy budget rather than a calibrated accretion timescale. Increasing core mass generally facilitates faster gas growth in the appropriate envelope regime. The [critical core mass for gas accretion](../../../../critical-core-mass-for-gas-accretion.md) depends on [opacity](../../../../opacity.md), solid accretion heating and disk conditions; no one exact threshold follows from the histogram. If envelope cooling becomes rapid enough and gas supply persists, [runaway gas accretion](../../../../runaway-gas-accretion.md) can produce a giant. If core growth or cooling is too slow, [protoplanetary disk dispersal](../../../../protoplanetary-disk-dispersal.md) removes the reservoir first, leaving a rocky core or a smaller planet with a limited envelope.

The [snow line](../../../../snow-line.md) changes the supply of condensed solids: where water ice can survive, additional solid material can help cores grow. Its location depends on the evolving disk [temperature](../../../../temperature-split.md) and [pressure](../../../../pressure-split.md), so there is no universal orbital radius at which giants must form. Short-period planets need not have assembled entirely at their present locations. [Planetary migration](../../../../planetary-migration.md) can carry cores and giants inward; scattering and collisions can further reshape their [orbits](../../../../orbit-dynamical-system.md). [Pebble accretion](../../../../pebble-accretion.md) is another way to supply solids rapidly to embryos, but its efficiency depends on particle coupling and the available pebble flow. These processes alter the distribution without requiring every core to become a giant.

Radius also is not a linear proxy for [mass](../../../../mass.md). A relatively small [hydrogen](../../../../hydrogen.md)-[helium](../../../../helium.md) envelope can increase a planet's [radius](../../../../radius.md) substantially, so some planets with a few [Earth](../../../../earth.md) radii need not be purely rocky. Contraction as planets cool and irradiation-driven [atmospheric escape](../../../../atmospheric-escape.md) can subsequently reduce their radii. Hence the final histogram combines solid growth, gas capture, migration and later thermal evolution. In particular, the smallest bins need not all share one composition or one formation location.

Direct fragmentation through [gravitational instability of an astrophysical disk](../../../../gravitational-instability-of-an-astrophysical-disk-split.md) is an alternative route to massive gaseous objects. It requires a sufficiently self-gravitating disk, described locally by [Toomre's stability criterion](../../../../toomre-s-stability-criterion.md), together with sufficiently rapid cooling for bound fragments to survive. It does not naturally explain the dominant population of small close-in cores by itself, although migration or further evolution can change the locations of fragments. The observed abundance of small planets is therefore consistent with solid cores commonly forming while only a minority acquire a massive gas envelope before disk dispersal. It does not uniquely prove a particular prescription for each uncertain growth stage.

**The physical explanation is widespread core formation combined with restricted access to runaway gas accretion.** The strongest observational conclusion concerns small versus giant planets in the stated period range, after accounting for selection; the figure alone does not determine a universal core threshold, a unique mass distribution, or the population beyond the period cut.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the exoplanets and Planetary Systems course of the University of Cambridge](../../../split.md)
5. [Exoplanets and Planetary Systems course of the University of Cambridge](../../../../exoplanets-and-planetary-systems-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
