<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

**Two interface effects.** For $n_2<n_1$, [Snell's law](../../../../../snell-s-law.md) gives $\sin\theta_t=(n_1/n_2)\sin\theta_i$. If $\sin\theta_i>n_2/n_1$, no propagating transmitted ray exists: there is [total internal reflection](../../../../../total-internal-reflection.md), with an [evanescent wave](../../../../../evanescent-wave.md) on the far side. An [optical fibre](../../../../../optical-fiber.md) uses this to guide light.

For ordinary isotropic nonmagnetic media, $\tan\theta_i=n_2/n_1$ is the [Brewster angle](../../../../../brewster-s-angle.md). The reflected p-polarized component, whose electric field lies in the incidence plane, vanishes; the reflected s-polarized component generally remains. Reflection polarizers and polarized glare reduction exploit this selectivity.

**The plasma response.** Neglect collisions, thermal-pressure corrections and background magnetic field. Let the wave vary as $e^{-i\omega t}$. An electron displacement obeys

$$
-m_e\omega^2\mathbf x_e=-e\mathbf E,\qquad
\mathbf x_e=\frac{e\mathbf E}{m_e\omega^2}.
$$

Its dipole moment is $-e\mathbf x_e$, so the electron [electric polarization](../../../../../polarization-density.md) is $\mathbf P_e=-ne^2\mathbf E/(m_e\omega^2)$. Ions of charge $Ze$ give a further contribution $\mathbf P_i=-nZe^2\mathbf E/(m_i\omega^2)$, smaller by $Zm_e/m_i$. Thus heavy ions move negligibly at these electron-wave frequencies. Using $\mathbf D=\varepsilon_0\mathbf E+\mathbf P$ gives the [cold collisionless plasma dielectric response](../../../../../cold-collisionless-plasma-dielectric-response.md),

$$
\boxed{\varepsilon_r=1-\frac{\omega_p^2}{\omega^2},\qquad
\omega_p^2=\frac{ne^2}{m_e\varepsilon_0}.}
$$

For this model $\mu_r\simeq1$, so $n_{\rm refr}^2=\varepsilon_r$ and $c^2k^2=\omega^2-\omega_p^2$ for the transverse [electromagnetic wave](../../../../../electromagnetic-wave-split.md).

**The vertical cutoff and density.** Below the [plasma frequency](../../../../../plasma-frequency.md), the squared refractive index is negative: the wave is an [evanescent wave](../../../../../evanescent-wave.md) instead of propagating through a layer hundreds of kilometres thick. The observed $5\ \mathrm{MHz}$ cutoff therefore identifies $f_p=5.0\times10^6\ \mathrm{Hz}$, with $\omega_p=2\pi f_p$. Consequently

$$
\boxed{n=\frac{\varepsilon_0m_e(2\pi f_p)^2}{e^2}
\simeq3.10\times10^{11}\ \mathrm{m^{-3}}.}
$$

This uses $\varepsilon_0=8.854\times10^{-12}\ \mathrm{F\,m^{-1}}$, $m_e=9.109\times10^{-31}\ \mathrm{kg}$ and $e=1.602\times10^{-19}\ \mathrm C$. The density is also $3.10\times10^5\ \mathrm{cm^{-3}}$.

**The transmission elevation.** At $f=8\ \mathrm{MHz}$, the [ionosphere](../../../../../ionosphere.md) has refractive index

$$
n_i=\sqrt{1-\left(\frac58\right)^2}
=\frac{\sqrt{39}}8\simeq0.7806.
$$

If $\alpha$ is elevation above horizontal, incidence at the layer is $\theta_i=\pi/2-\alpha$. Avoiding [total internal reflection](../../../../../total-internal-reflection.md) requires $\sin\theta_i=\cos\alpha<n_i$. The limiting elevation is therefore

$$
\boxed{\alpha_{\min}=\arccos n_i=\arcsin(5/8)\simeq38.7^\circ.}
$$

Strictly, it must point above this limiting angle to carry upward power through the finite layer: at equality the transmitted wave is grazing. With a suitable satellite position, the stated orbital altitude imposes no additional angular constraint in this flat-layer approximation.

**Polarization-selective ground reflection.** The ray's incidence plane is vertical. Horizontal electric polarization is s polarization; the other transverse polarization lies in the vertical incidence plane and is p polarization. Reflection of s but not p identifies the [Brewster angle](../../../../../brewster-s-angle.md), not [total internal reflection](../../../../../total-internal-reflection.md), which would reflect both in this lossless isotropic model. Thus

$$
\tan\theta_B=n_i,\qquad \theta_B\simeq38.0^\circ.
$$

For a reflecting height $h=200\ \mathrm{km}$, the horizontal range consists of two equal legs. The [Brewster reflection from an ionospheric interface](../../../../../brewster-reflection-from-an-ionospheric-interface.md) gives

$$
\boxed{D=2h\tan\theta_B=400\,n_i\ \mathrm{km}
\simeq312\ \mathrm{km}.}
$$

At this angle $\theta_B$ is below the critical incidence angle, so a transmitted ray also exists; the detected horizontal component is an ordinary partial reflection. The s-polarized reflected power fraction is approximately $[(1-n_i^2)/(1+n_i^2)]^2\simeq0.059$, whereas the ideal p-polarized reflected fraction is zero. These results use the question's sharp planar interface model and exclude upper-interface reflections.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
