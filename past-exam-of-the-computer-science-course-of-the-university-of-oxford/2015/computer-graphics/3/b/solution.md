<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [bidirectional reflectance distribution function](../../../../../bidirectional-reflectance-distribution-function.md), or [BRDF](../../../../../bidirectional-reflectance-distribution-function.md), describes how a surface scatters incident illumination into each outgoing direction. At a fixed surface [point](../../../../../point-geometry.md) $p$ and [wavelength](../../../../../wavelength.md), its inputs are two directions above the surface, $\omega_i$ toward the incident source and $\omega_o$ toward the observer; equivalently these are two pairs of angular coordinates. Its output is the ratio of differential reflected [radiance](../../../../../radiance.md) to differential incident [irradiance](../../../../../irradiance.md):

$$
\boxed{f_r(p,\omega_i,\omega_o)=\frac{dL_o(p,\omega_o)}{dE_i(p,\omega_i)},\qquad [f_r]=\mathrm{sr}^{-1}.}
$$

Position and [wavelength](../../../../../wavelength.md) may be additional arguments when material properties vary. A colour implementation can return one value per colour channel. The [BRDF](../../../../../bidirectional-reflectance-distribution-function.md) is a material response, not the final outgoing light value: it must be combined with the incident illumination and the projected-angle factor.[§4.3.1, definition of the BRDF as differential outgoing radiance divided by differential incident irradiance](../../../../../physically-based-rendering-from-theory-to-implementation-4th-edition-by-matt-pharr-and-others.md)

For incident [radiance](../../../../../radiance.md) $L_i$, the reflection part of the [rendering equation](../../../../../rendering-equation.md) is

$$
L_o(p,\omega_o)=\int_{\Omega^+}f_r(p,\omega_i,\omega_o)L_i(p,\omega_i)(\hat N\cdot\omega_i)\,d\omega_i.
$$

Emission is added separately if the surface itself emits. This integral explains how a [BRDF](../../../../../bidirectional-reflectance-distribution-function.md) replaces the assumed material response of a local lighting model. For [Lambertian reflectance](../../../../../lambertian-reflectance.md), $f_r=\rho_d/\pi$, so the cosine factor yields the diffuse term from part (a). A directional specular lobe supplies a highlight. The empirical [Phong reflection model](../../../../../phong-reflection-model.md) is an approximate angular-response model of this kind; its original direct specular term is not automatically a normalized, energy-conserving [BRDF](../../../../../bidirectional-reflectance-distribution-function.md). The ambient term approximates missing illumination and is not itself a third direction-independent material scattering mechanism. More general [BRDFs](../../../../../bidirectional-reflectance-distribution-function.md) can reproduce measured surface behaviour, while illumination from other surfaces supplies indirect light in the [rendering equation](../../../../../rendering-equation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Computer graphics](../../../computer-graphics-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
