<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Many open-ocean [chlorophyll retrieval](../../../../../chlorophyll-retrieval.md) algorithms infer [chlorophyll a](../../../../../chlorophyll-a.md) from the blue-to-green [remote-sensing reflectance](../../../../../remote-sensing-reflectance.md) ratio. Increasing pigment generally depresses blue reflectance relative to green. In coastal waters, however, [coloured dissolved organic matter](../../../../../coloured-dissolved-organic-matter.md) and [non-algal particles](../../../../../non-algal-particle.md) can independently absorb blue light, as in the sketches, and therefore mimic an increase in pigment. Their concentrations need not covary with [phytoplankton biomass](../../../../../phytoplankton-biomass.md): river runoff and sediment resuspension can change them separately.

Moreover, the satellite measures emerging [radiance](../../../../../radiance.md), not absorption directly. Schematically,

$$
R_{rs}(\lambda)\propto\frac{b_b(\lambda)}{a(\lambda)+b_b(\lambda)},
$$

where $b_b$ is the [backscattering coefficient](../../../../../backscattering-coefficient.md); this is an explanatory approximation, not a complete retrieval formula. Suspended particles change both absorption and backscattering, and different mixtures can produce similar band ratios. Shallow-bottom reflection, land-adjacency effects and more difficult [atmospheric correction](../../../../../atmospheric-correction.md) introduce further coastal errors. Consequently a simple blue/green ratio can overestimate [chlorophyll a](../../../../../chlorophyll-a.md) when excess CDOM removes blue light, although sediment scattering and other effects mean the bias is not universally positive. Multiband or hyperspectral methods that separately constrain pigment, dissolved absorption and particles, supported by local observations, are preferable in optically complex water.[Revision 4, Volume I: unaccounted blue absorption by CDOM creates regional chlorophyll-retrieval uncertainty; absorption and scattering are distinct optical properties.](../../../../../ocean-optics-protocols-for-satellite-ocean-color-sensor-validation-revision-4-volume-i-by-nasa.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2025](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
