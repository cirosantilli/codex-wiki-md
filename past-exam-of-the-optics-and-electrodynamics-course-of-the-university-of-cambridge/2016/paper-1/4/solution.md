<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Spherical-particle [frequency](../../../../frequency.md) scaling.** For a [dielectric](../../../../dielectric.md) sphere of radius $a\ll\lambda$, the quasistatic [electric polarizability](../../../../electric-polarizability.md) is

$$
\alpha_s=4\pi\epsilon_0a^3\frac{\epsilon_r-1}{\epsilon_r+2},\qquad\mathbf p(t)=\operatorname{Re}(\alpha_s\mathbf E_0e^{-i\omega t}).
$$

The [electric dipole radiation](../../../../electric-dipole-radiation.md) formula and $I_0=\epsilon_0c|E_0|^2/2$ give

$$
\langle P\rangle=\frac{\omega^4|\alpha_s|^2|E_0|^2}{12\pi\epsilon_0c^3},\qquad\boxed{\sigma=\frac{\langle P\rangle}{I_0}=\frac{8\pi}{3}k^4a^6\left|\frac{\epsilon_r-1}{\epsilon_r+2}\right|^2.}
$$

Thus **[Rayleigh scattering](../../../../rayleigh-scattering.md) scales as $\omega^4$, or $\lambda^{-4}$**, when the polarizability varies slowly with [frequency](../../../../frequency.md). Material resonances and absorption can change this simple scaling. For the incident $z$ [polarization](../../../../polarization-waves.md), the dipole is along $z$: intensity is proportional to $\sin^2\chi$, where $\chi$ is the angle from $z$. There is no radiation on the dipole axis and a maximum in the $xy$ plane. In a direction $\hat{\mathbf n}$ the scattered [electric field](../../../../electric-field-split.md) is along $\hat{\mathbf z}-(\hat{\mathbf z}\cdot\hat{\mathbf n})\hat{\mathbf n}$, hence linearly polarized wherever nonzero.[Small-particle dipole response and inverse-fourth-power wavelength dependence](../../../../rayleigh-scattering-by-richard-fitzpatrick.md)

<a id="4/image-a-z-directed-electric-dipole-radiates-most-strongly-perpendicular-to-its-axis-and-has-axial-zeros"></a>
![](../../../../past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2016/paper-1-rayleigh-pattern.png)

**[Figure 5](#4/image-a-z-directed-electric-dipole-radiates-most-strongly-perpendicular-to-its-axis-and-has-axial-zeros). A z-directed electric dipole radiates most strongly perpendicular to its axis and has axial zeros**. [Source](paper-1-rayleigh-pattern.py).

**Needle model used in parts (a)–(d).** Let its axis be $\mathbf u=(u_x,u_y,u_z)=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta)$. A very slender, high-permittivity needle has dominant longitudinal response, so use the [rank-one needle polarizability](../../../../rank-one-needle-polarizability.md) $\boldsymbol\alpha\simeq\alpha_\parallel\mathbf u\mathbf u^{\mathsf T}$. Its transverse response is neglected at leading order. For observation along $y$, define $\mathbf v=u_x\hat{\mathbf x}+u_z\hat{\mathbf z}$, $s=|\mathbf v|^2=1-u_y^2$ and

$$
K=\frac{k^4|\alpha_\parallel|^2}{16\pi^2\epsilon_0^2R^2}.
$$

For a unit incident [Jones vector](../../../../jones-vector.md) $\mathbf e$, the common far-field relation is $\mathbf E_s\propto\mathbf v(\mathbf u\cdot\mathbf e)$, and $I_s=KI_0s|\mathbf u\cdot\mathbf e|^2$. Here $I_s$ is irradiance at distance $R$; multiplying by $R^2$ gives power per solid angle. No absolute value of $\alpha_\parallel$ is given or needed for the requested relative intensities.

**Diffuse random cloud, with the incident [polarization](../../../../polarization-waves.md) of (a).** The single-particle amplitudes through $x$ and $z$ analysers are proportional to $u_xu_z$ and $u_z^2$. The [isotropic orientation fourth moment](../../../../isotropic-orientation-fourth-moment.md) gives the [needle-scattering analyzer moments](../../../../needle-scattering-analyzer-moments.md)

$$
\langle u_x^2u_z^2\rangle=\frac1{15},\qquad\langle u_z^4\rangle=\frac15.
$$

For example, $\langle u_z^4\rangle=\tfrac12\int_{-1}^{1}\mu^4d\mu=1/5$; symmetry and $u_x^2+u_y^2+u_z^2=1$ give $2\langle u_x^2u_z^2\rangle=1/3-1/5$. Since the particles scatter mutually incoherently, intensities add. For $N$ illuminated particles,

$$
\boxed{I_x=\frac{NKI_0}{15},\qquad I_z=\frac{NKI_0}{5},\qquad I_x:I_z=1:3.}
$$

The cross correlation vanishes by reflection symmetry. The degree of [linear polarization](../../../../linear-polarization.md) is $(I_z-I_x)/(I_z+I_x)=\boxed{1/2}$: random anisotropic scatterers produce partially depolarized light, even though every individual needle produces a single [linear polarization](../../../../linear-polarization.md).

<a id="4/image-independent-isotropically-oriented-needles-give-the-analyser-ratio-one-to-three-while-coherent-mean-amplitudes-have-no-x-component"></a>
![](../../../../past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2016/paper-1-needle-ensemble.png)

**[Figure 6](#4/image-independent-isotropically-oriented-needles-give-the-analyser-ratio-one-to-three-while-coherent-mean-amplitudes-have-no-x-component). Independent isotropically oriented needles give the analyser ratio one to three, while coherent mean amplitudes have no x component**. [Source](paper-1-needle-ensemble.py).

**Continuous homogeneous [dielectric](../../../../dielectric.md).** One must sum amplitudes coherently and include their spatial phases, rather than retain the preceding sum of intensities. Random orientations give $\langle\mathbf u\mathbf u^{\mathsf T}\rangle=\mathbf I/3$, so the averaged response is isotropic and its induced [polarization](../../../../polarization-waves.md) is along $z$. Its coherent radiation toward $y$, when allowed by the sample geometry, is therefore **purely $z$ polarized, with $I_x=0$**. The independent-needle prefactor is no longer a quantitative dense-medium model; local-field and collective effects determine the effective [permittivity](../../../../permittivity-split.md).

There is also [coherent continuum phase matching](../../../../coherent-continuum-phase-matching.md): a uniform bulk driven by a [plane wave](../../../../plane-wave.md) has no arbitrary outgoing $90^\circ$ plane-wave component. In an ideal infinite homogeneous medium there is no diffuse side scattering at all; propagation, [refraction](../../../../refraction.md) and reflection are determined by the medium and its interfaces. A finite sample's coherent side signal depends on its shape and boundaries. Thus the old $1:3$ diffuse ratio is replaced by a coherent isotropic-medium response, not by a universal nonzero $N^2$ side-scattering intensity.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
5. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
