<h1 id="s10/1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [CT number](../../../../../ct-number.md) is a dimensionless relative attenuation measure, conventionally $H=1000(\mu_{\rm CT}-\mu_{{\rm water},\rm CT})/\mu_{{\rm water},\rm CT}$. The [X-ray](../../../../../x-ray.md) spectrum used in [computed tomography](../../../../../computed-tomography.md) has an effective energy far below $511\,\mathrm{keV}$ and is polychromatic. Its [photoelectric absorption](../../../../../photoelectric-absorption.md) contribution depends strongly on composition, whereas water and soft-tissue attenuation at the [positron emission tomography](../../../../../positron-emission-tomography.md) energy is mainly [Compton scattering](../../../../../compton-scattering.md). Thus a [CT number](../../../../../ct-number.md) is neither a $511\,\mathrm{keV}$ [linear attenuation coefficient](../../../../../linear-attenuation-coefficient.md) nor an energy-independent [mass attenuation coefficient](../../../../../mass-attenuation-coefficient.md).

The usual conversion calibrates a piecewise linear or bilinear relation between [CT numbers](../../../../../ct-number.md) and $\mu(511\,\mathrm{keV})$. The air–water branch models predominantly density differences in lung and soft tissue; a separate water–bone branch accounts for the different energy dependence of mineralized tissue. The calibration depends on the [computed tomography](../../../../../computed-tomography.md) spectrum. After geometric registration, the resulting [linear attenuation coefficient](../../../../../linear-attenuation-coefficient.md) map is forward projected along each [coincidence line of response](../../../../../coincidence-line-of-response.md) to obtain $\exp(\int\mu_{511}\,ds)$. If a mass coefficient is stored, its conversion to a linear coefficient must also include [mass density](../../../../../density.md). Unusual high-atomic-number materials can violate the simple tissue calibration, so the conversion is a physical material model, not a universal arithmetic rescaling.[original study: segmentation, scaling and hybrid conversion from CT energies to 511 keV](../../../../../attenuation-correction-for-a-combined-3d-pet-ct-scanner-by-paul-e-kinahan-and-others.md)[Materials and Methods: piecewise conversion and air–water versus water–bone mixture branches](../../../../../accuracy-of-ct-based-attenuation-correction-in-pet-ct-bone-imaging-by-monica-abella-and-others.md)

## ↑ Ancestors (12)

1. [3](../3.md)
2. [1](../../1.md)
3. [S10](../../../s10.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
