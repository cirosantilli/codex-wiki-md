<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Ignoring [refraction](../../../../refraction.md), the line of sight is perpendicular to the radius at its tangent point. For a surface tangent, [Pythagorean theorem](../../../../pythagorean-theorem.md) gives the satellite-to-tangent distance

$$
\boxed{D=\sqrt{(R+H)^2-R^2}
=\sqrt{7171^2-6371^2}\,\mathrm{km}
=3291\,\mathrm{km}\simeq3300\,\mathrm{km}.}
$$

For tangent altitude $z_t$, replace $R^2$ by $(R+z_t)^2$; lower [atmospheric scale heights](../../../../atmospheric-scale-height.md) change the estimate little. The required angular resolution is

$$
\theta\simeq\frac{8.5\,\mathrm{km}}{3291\,\mathrm{km}}
=2.58\times10^{-3}\,\mathrm{rad}.
$$

Using the [Rayleigh criterion](../../../../rayleigh-criterion.md) for a circular telescope aperture, $\theta=1.22\lambda/d$. The longest [wavelength](../../../../wavelength.md) imposes the strongest condition, so

$$
\boxed{d_{\rm diffraction}\gtrsim
\frac{1.22(20\times10^{-6}\,\mathrm m)}{2.58\times10^{-3}}
=9.45\times10^{-3}\,\mathrm m\simeq9.5\,\mathrm{mm}.}
$$

The corresponding requirement at $7\,\mu\mathrm m$ is $3.3$ mm. This is a [diffraction](../../../../diffraction.md) limit, without allowance for scan sampling, aberrations or instrumental field of view.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
