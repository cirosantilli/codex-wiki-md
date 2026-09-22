<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**A defensible period design answer for [hospital bed space](../../../../../hospital-bed-space.md) is roughly 1,600 cubic feet, or 45 cubic metres, per bed in a properly ventilated ordinary ward. This is a volume allowance, not a ventilation rate or a universal legal minimum.** In the 1863 third edition of [Notes on Hospitals by Florence Nightingale](../../../../../notes-on-hospitals-by-florence-nightingale.md), [Florence Nightingale](../../../../../florence-nightingale.md) gives a twenty-patient ward measuring 80 by 25 by 16 feet, or alternatively 80 by 26 by 15 feet. These examples give 1,600 or 1,560 cubic feet per bed, respectively.[Third edition, 1863, p.67, “Principles of Hospital Construction”, example ward dimensions and cubic space](../../../../../notes-on-hospitals-by-florence-nightingale.md)

For the first arrangement,

$$
\boxed{\frac{V}{N}=\frac{80\times25\times16}{20}=1600\ \mathrm{ft^3}\simeq45.3\ \mathrm{m^3}\text{ per bed}.}
$$

This is a cited design example, not a measurement of an unseen ward. Floor area, separation between beds, access for nursing, air distribution and the condition of the patients also matter. Simply adding height cannot compensate for crowding patients together or leaving stagnant zones around the beds. A modern hospital would apply its current design and infection-control requirements rather than treat the 1863 figure as sufficient for every clinical purpose.

To determine [hospital ward ventilation](../../../../../hospital-ward-ventilation.md), first measure the ward's internal volume $V$. Measure the area $A$ of each effective inlet or outlet and the mean normal [velocity](../../../../../velocity.md) $\bar u$ across it, using an [anemometer](../../../../../anemometer.md) and several positions rather than one favourable point. The volume flow is $Q=A\bar u$, or the sum of the flows through independent openings of the same side of the balance. Do not add both the incoming and outgoing flow and call their sum new air. Reverse flow, leakage, changes of wind and temperature, and recirculation must be considered. Smoke may reveal direction and stagnant regions, but its visible movement alone is not a quantitative flow measurement. Modern institutional instrument guidance also explains why velocity must be sampled across a section; the simple area–velocity relation itself does not depend on a modern electronic instrument.[“How to Calculate Airflow Rate from a Velocity Probe Measurement”: spatial sampling, mean velocity and suitable instruments](../../../../../measuring-mechanical-ventilation-airflow-by-pacific-northwest-national-laboratory.md)

With $Q$ expressed per hour, the mean [air changes per hour](../../../../../air-change-rate.md) are

$$
\boxed{a=\frac{Q}{V},\qquad q_{\text{bed}}=\frac{Q}{N}.}
$$

The quantities have different meanings: $V/N$ is space per bed, $Q/N$ is fresh-air supply per bed per hour, and $a$ is the nominal exchange rate. A system may move much recirculated [air](../../../../../air.md) while supplying relatively little new outdoor [air](../../../../../air.md).

A second method is to follow the fall of a [tracer gas](../../../../../tracer-gas.md) after its source stops. Under a well-mixed, constant-flow model with constant outdoor concentration $C_o$ and no continuing internal generation,

$$
\frac{d(C-C_o)}{dt}=-\frac{Q}{V}(C-C_o),
\qquad
\boxed{a=\frac{\ln[(C_1-C_o)/(C_2-C_o)]}{t_2-t_1}.}
$$

Here time is in hours if $a$ is to be reported per hour. The formula follows by integrating the mass balance. Compare measurements at several positions and state the conditions. Poor mixing, continuing generation by occupants and changing wind invalidate a simple one-exponential interpretation. Current institutional guidance describes this decay method; the modern monitoring protocol is a later comparison, while the elementary balance explains what “rate of change” measures.[2020, overview and protocol: cessation of source, concentration decay, background and dependence on conditions](../../../../../air-change-rate-input-parameter-protocol-by-the-world-health-organization.md)

The ordinary ward impurities to examine are excess [carbon dioxide](../../../../../carbon-dioxide.md) and [water vapour](../../../../../water-vapor.md) from occupants, volatile material including [Ammonia](../../../../../ammonia.md), organic and inorganic dust, and potentially infectious [aerosols](../../../../../aerosol.md). [Carbon monoxide](../../../../../carbon-monoxide.md) or irritant combustion gases may enter where heating or lighting is defective; drain-associated gases are a contingent additional hazard, not something necessarily present in every ward. Record occupancy, combustion sources, windows, sampling position, temperature and time, and take an outdoor comparison sample.

For [carbon dioxide](../../../../../carbon-dioxide.md), collect a known volume of [air](../../../../../air.md) in a calibrated vessel and expose it to a measured amount of standardized [barium hydroxide](../../../../../barium-hydroxide.md). Absorption produces [barium carbonate](../../../../../barium-carbonate.md). Compare the remaining alkali with a reagent blank, excluding carbonate precipitate from an acid titration that would dissolve it. The consumed alkali gives the absorbed [carbon dioxide](../../../../../carbon-dioxide.md); express that amount per original volume of [air](../../../../../air.md). A report from 1864 describes the method in 7–10 litre globes with a gravimetric comparison, establishing a procedure available before the examination.[p.80, “Note on the Amount of Carbonic Acid contained in the Air of Manchester”: baryta absorption and gravimetric check](../../../../../chemical-news-volume-9-1864.md)

Estimate humidity with wet- and dry-bulb thermometers, or gravimetrically by collecting moisture in a weighed drying absorber from a measured volume of [air](../../../../../air.md). For volatile bases, pass a measured sample through dilute acid and determine the uptake, interpreting possible [Ammonia](../../../../../ammonia.md) alongside interfering bases. Mere change of [litmus](../../../../../litmus.md) is a screen, not a selective low-concentration quantitative assay. A modern example uses acid-treated collection medium and [ion chromatography](../../../../../ion-chromatography.md), with calibrated sampling and blanks; that later analytical specification must not be credited to 1865.[Sampling and measurement: collected ammonia, air volume, blanks and instrumental determination](../../../../../ammonia-by-ion-chromatography-method-6016-by-the-national-institute-for-occupational-safety-and-health.md)

Collect suspended material on a suitable filter or surface and examine it by [microscopy](../../../../../microscopy.md); a controlled gravimetric collection gives particle mass per volume. Such measurements do not by themselves identify pathogens or count every inhalable organism. Period assessments also used [potassium permanganate](../../../../../potassium-permanganate.md) decolourization to investigate oxidizable contamination. The 1865 chemical press already warned that other reducing substances could decolourize it, so a supposed “organic matter” result was nonspecific.[14 April, p.179, review of air in mines and confined places: limitations of permanganate as an organic-matter estimate](../../../../../chemical-news-volume-11-1865.md)

Finally, report chemical cleanliness, particle loading and ventilation performance separately. They are related aspects of ward conditions, but one cannot derive freedom from infection from a low [carbon dioxide](../../../../../carbon-dioxide.md) result or a weak smell. Modern infection-control guidance similarly emphasizes that microbial air samples depend on collection method, location, timing and an interpretable sampling plan.[Air sampling, comparison conditions, method limitations and interpretation of results](../../../../../environmental-sampling-by-the-centers-for-disease-control-and-prevention.md)

## ↑ Ancestors (11)

1. [4](../4.md)
2. [Forensic medicine and hygiene](../../forensic-medicine-and-hygiene-split.md)
3. [Second examination](../../split.md)
4. [1865](../../../split.md)
5. [Past exam of the medicine course of the University of Oxford](../../../../split.md)
6. [Medicine course of the University of Oxford](../../../../../medicine-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
