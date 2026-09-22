<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Post-receptoral processing compares cone signals, organizes those comparisons across space and time, and uses them to represent surfaces and objects. Three receptor classes do not imply three [neurons](../../../neuron-split.md) labelled with three [color](../../../color.md) names.** A complete answer must distinguish the information available at the receptors from its neural transformation and its perceptual interpretation.

The [principle of univariance](../../../principle-of-univariance.md) supplies the starting constraint. For one cone class, an absorption-dependent response does not identify [wavelength](../../../wavelength.md) independently of [intensity](../../../intensity-physics.md). Comparing differently sensitive classes makes chromatic information available. Relative to an adapted background, cone contrasts can be written $c_j=(Q_j-Q_{j0})/Q_{j0}$, where $Q_{j0}>0$ is the background catch. This representation separates a change relative to the prevailing input from the raw number of absorbed [photons](../../../photon.md). It is a useful coordinate system, not a claim that every [neuron](../../../neuron-split.md) implements this exact formula.

Retinal circuitry immediately transforms the signals. [Light](../../../light.md) hyperpolarizes [cone cells](../../../cone-cell.md) and changes their transmitter release. ON and OFF bipolar pathways respond differently to changes in cone output, while horizontal and amacrine circuitry contribute spatial and temporal interactions. [Retinal ganglion cells](../../../retinal-ganglion-cell.md) transmit [spike trains](../../../spike-train.md) rather than simply forwarding a cone's voltage. Their center–surround organization compares regions, so chromatic and spatial structure are already intertwined. Near the central [retina](../../../retina.md), the midget pathway can oppose an L- or M-dominated center to a surround containing other cone input. The same circuitry can carry information useful for fine spatial structure and for chromatic contrast; these are not necessarily separate wires.

A distinct S-cone route illustrates the anatomical specificity. [Dennis M. Dacey](../../../dennis-m-dacey.md) and colleagues combined physiological characterization with identification of ganglion-cell morphology in primate [retina](../../../retina.md), finding that the S-ON opponent response belonged to a small bistratified ganglion-cell type rather than simply another midget cell.[Nature 367, 731–735; physiological and morphological identification](../../../the-blue-on-opponent-pathway-in-primate-retina-originates-from-a-distinct-bistratified-ganglion-cell-type-by-dennis-m-dacey-and-others.md) This supports parallel circuits with different cone combinations. Calling the pathway “blue-on” is shorthand for its stimulus response, not proof that the cell itself produces a unique blue experience.

At a simplified computational level, an achromatic-like combination and two chromatic combinations can be represented as

$$
y_0=c_L+c_M,\qquad y_1=c_L-c_M,\qquad y_2=c_S-\tfrac12(c_L+c_M).
$$

This [invertible three-channel opponent transform](../../../invertible-three-channel-opponent-transform.md) reorganizes three coordinates rather than creating additional independent spectral information. Their [matrix](../../../matrix.md) has [determinant](../../../determinant.md) $-2$, so the transform is invertible: $c_L=(y_0+y_1)/2$, $c_M=(y_0-y_1)/2$ and $c_S=y_2+y_0/2$. Actual weights depend on cell, location, adaptation and stimulus conditions. This algebra is an illustrative opponent transform, not a fitted retinal wiring diagram or a complete perceptual [color space](../../../color-space.md).

The [lateral geniculate nucleus](../../../lateral-geniculate-nucleus.md) preserves several parallel retinal pathways while also participating in cortical interactions. [A. M. Derrington](../../../a-m-derrington.md) and colleagues studied macaque geniculate cells with gratings whose [luminance](../../../luminance.md) and chromatic modulation could be varied independently on a calibrated [color](../../../color.md) television display. Finding directions that changed cone stimulation without driving a cell constrained its linear cone weights.[J Physiol 357, 241–265; null-plane method and chromatic stimulus space](../../../chromatic-mechanisms-in-lateral-geniculate-nucleus-of-macaque-by-a-m-derrington-and-others.md) For a nonzero linear weight vector, the zero-response contrasts obey $r=\mathbf w^{\mathsf T}\mathbf c=0$, defining a [chromatic null plane](../../../chromatic-null-plane.md). A null response therefore tests a relation between inputs, rather than merely assigning the cell a preferred [color](../../../color.md) name. The resulting opponent directions need not coincide with human [unique hues](../../../unique-hue.md).

Cortical processing adds more complex spatial comparisons. [Bevil R. Conway](../../../bevil-conway.md) mapped cone inputs to color-responsive [neurons](../../../neuron-split.md) in alert macaque V1 using cone-isolating spots and eye-position-corrected reverse correlation. Some cells combined chromatic opponency with opposite tuning in adjacent spatial subregions.[J Neurosci 21, 2768–2783; receptive-field mapping and double opponency](../../../spatial-structure-of-cone-inputs-to-color-cells-in-alert-macaque-primary-visual-cortex-by-bevil-r-conway.md) Such [double-opponent cells](../../../double-opponent-cell.md) can respond strongly to a chromatic boundary while responding less to a spatially uniform change. This offers a mechanism useful for separating surface differences from shared illumination changes. It does not establish that one V1 population alone solves [color constancy](../../../color-constancy.md) under arbitrary scenes.

Further processing must relate [color](../../../color.md) to form, illumination, material and the current task. The same cone contrasts can be interpreted differently in a shadow, highlight or translucent object. Surface [color](../../../color.md) judgments, discrimination thresholds and [color naming](../../../color-naming.md) therefore constrain different computations. Feedback and [attention](../../../attention.md) can influence which information is selected, while [learning](../../../learning.md) can alter how a signal is interpreted or normalized. A lesion or imaging response can constrain contributions to those tasks, but an area responsive to [color](../../../color.md) is not automatically an isolated “[color](../../../color.md) center.”

The strongest picture is consequently a hierarchy of interacting computations: cone-specific signals, opponent and spatial filtering, combinations tuned to richer image structure, and object-level judgments. **Trichromatic sampling limits spectral information; later processing determines how that information supports boundaries, stable surface appearance and behavior.**

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2022](../../2022-split.md)
3. [Past exam of the sensing and perceiving light, colour and materials course of the University of Oxford](../../split.md)
4. [Sensing and perceiving light, colour and materials course of the University of Oxford](../../../sensing-and-perceiving-light-colour-and-materials-course-of-the-university-of-oxford.md)
5. [Year 3 of the psychology (experimental) course of the University of Oxford](../../../year-3-of-the-psychology-experimental-course-of-the-university-of-oxford.md)
6. [Psychology (experimental) course of the University of Oxford](../../../psychology-experimental-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
