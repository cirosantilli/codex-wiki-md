<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**[Photoreceptors](../../../photoreceptor.md) determine which optical differences are available for vision, with what noise and spatial–temporal precision. They strongly constrain [light](../../../light.md), [color](../../../color.md) and [material perception](../../../material-perception.md) without uniquely determining the eventual percept.** Later processing can exploit context and action, but cannot recover arbitrary information already lost in receptor sampling.

For cone class $j$, a simplified expected quantum catch over one sampling interval is

$$
Q_j=\int N(\lambda)a_j(\lambda)\,d\lambda,
$$

where $N$ is the incident photon-number spectrum at the receptor, including ocular filtering, and $a_j$ effective [absorption](../../../absorption-electromagnetic-radiation.md) [probability](../../../probability.md). An energy spectrum requires conversion by [photon](../../../photon.md) energy $hc/\lambda$ before this counting interpretation. The integral is many-to-one: equal catches do not imply equal spectra. The [principle of univariance](../../../principle-of-univariance.md) means that an individual receptor does not independently report [photon](../../../photon.md) [wavelength](../../../wavelength.md) and number.

Multiple receptor classes provide comparisons, but ordinary cone-mediated trichromacy still samples a spectral distribution with only three class responses at a specified location and time. In a discretized model, $\mathbf Q=A\mathbf n$ with three rows and more than three spectral bins. The [matrix](../../../matrix.md) has a nonzero [kernel](../../../kernel-of-a-linear-map-split.md). Around a strictly positive spectrum, a sufficiently small perturbation in that [kernel](../../../kernel-of-a-linear-map-split.md) preserves nonnegative intensities while leaving all three catches unchanged. This derives the possibility of [metamers](../../../metamer.md); it does not mean all real-world spectral differences are unobservable under every condition. Altering illumination, observer or spatial–temporal context can break a particular match.

Sensitivity also has a [photon](../../../photon.md) budget. In an ideal Poisson model, mean catch $N$ has [variance](../../../variance-split.md) $N$, so relative counting uncertainty is $1/\sqrt N$. Gathering more [photons](../../../photon.md) reduces this uncertainty but requires a larger effective collecting area or more integration time. Temporal averaging can obscure rapid change, while spatial pooling can sacrifice fine detail. Receptor and downstream noise add limitations beyond shot noise. Rods support low-light detection with different sensitivity and pooling from [cone cells](../../../cone-cell.md); if only one receptor class provides usable signals, [wavelength](../../../wavelength.md)–[intensity](../../../intensity-physics.md) ambiguity cannot be resolved by comparisons within that class. [Mesopic vision](../../../mesopic-vision.md), where rods and [cone cells](../../../cone-cell.md) can both contribute, is not captured by declaring all dim-light vision achromatic.

The receptor array is also uneven. [Christine A. Curcio](../../../christine-a-curcio.md) and colleagues mapped rods and [cone cells](../../../cone-cell.md) in whole-mounted human retinas using microscopic counts. Cone density was highest centrally and fell strongly with eccentricity, while the rod distribution differed and the central foveal region was rod-free.[J Comp Neurol 292, 497–523; methods and photoreceptor density maps](../../../human-photoreceptor-topography-by-christine-a-curcio-and-others.md) Thus acuity and sensitivity should not be treated as uniform over the visual field. Optical blur and downstream sampling constrain performance alongside receptor spacing. The S-cone mosaic is sparser than the combined L/M mosaic, so equal spatial detail cannot simply be assumed for all chromatic signals.

A regular one-dimensional model of [photoreceptor sampling](../../../photoreceptor-sampling.md) makes one limitation explicit. Sampling a sinusoid at spacing $d$ gives identical samples for frequencies $f$ and $f+k/d$, because the added phase at sample $n$ is $2\pi kn$. Restricting a real signal to frequencies below $1/(2d)$ avoids this basic [aliasing](../../../aliasing.md) ambiguity. Real retinal mosaics are two-dimensional, irregular and optically filtered, so this is a benchmark rather than a literal universal retinal cutoff. Fine material texture can consequently disappear or alias even when coarser [color](../../../color.md) and shape remain visible.

Individual variation changes the sampling system itself. [Heidi Hofer](../../../heidi-hofer.md) and colleagues' adaptive-optics measurements showed large L:M cone-ratio variation among observers passing normal [color](../../../color.md) tests.[J Neurosci 25, 9669–9679; retinal densitometry and corrected abstract](../../../organization-of-the-human-trichromatic-cone-mosaic-by-heidi-hofer-and-others.md) [Gabriele Jordan](../../../gabriele-jordan.md) and colleagues found behavioral evidence consistent with an extra chromatic dimension in one of a selected set of carriers with potential extra pigment diversity, rather than in every carrier.[J Vis 10(8):12; behavioral and genetic comparisons](../../../the-dimensionality-of-color-vision-in-carriers-of-anomalous-trichromacy-by-gabriele-jordan-and-others.md) These findings separate receptor availability from downstream use: receptor counts and pigment variants constrain possibilities without directly specifying appearance or functional dimensionality.

[Material perception](../../../material-perception.md) adds an inverse problem. For a matte surface under a single simplified [illuminant](../../../illuminant.md), the reflected [photon](../../../photon.md) spectrum is proportional to $E(\lambda)R(\lambda)$, so catches mix illumination and surface [reflectance](../../../reflectance.md). The same catches can therefore arise from different surfaces, even before considering three-channel spectral compression. [Specular reflection](../../../specular-reflection.md), [subsurface scattering](../../../subsurface-scattering.md), [translucency](../../../translucency.md) and [fluorescence](../../../fluorescence-split.md) introduce further dependencies on direction, geometry or [wavelength](../../../wavelength.md) conversion. Three cone values cannot independently label every physical material property.

Nevertheless, humans can exploit cues across space, movement and time. Highlights change with viewpoint; texture and shading constrain shape; surrounding surfaces provide illumination evidence. Such information can reduce ambiguity under useful assumptions, while metamerism and sampling limits remain. **Receptor properties define an information bottleneck and a set of trade-offs. Successful material recognition depends on combining what survives that bottleneck with contextual constraints, not on receptors directly measuring “wood,” “metal” or intrinsic surface [color](../../../color.md).**

## ↑ Ancestors (11)

1. [3](../3.md)
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
