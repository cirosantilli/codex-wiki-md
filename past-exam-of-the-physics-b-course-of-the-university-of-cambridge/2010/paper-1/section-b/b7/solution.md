<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

State a time convention before using complex response: take fields proportional to $e^{i(kz-\omega t)}$, with $k=k_r+i\kappa$ and $\kappa\geq0$ for a passive wave entering the material. In a homogeneous Ohmic medium, [Maxwell equations](../../../../../maxwell-equations-split.md) with $\mathbf J=\sigma\mathbf E$ give

$$
k^2=\mu\epsilon\omega^2+i\mu\sigma\omega
=\mu\omega^2\left(\epsilon+\frac{i\sigma}{\omega}\right).
$$

The [ohmic-conductor complex wavenumber](../../../../../ohmic-conductor-complex-wavenumber.md) describes both phase advance and [amplitude](../../../../../wave-amplitude.md) decay. Real constant conductivity is only a low-frequency approximation. In the [Drude model](../../../../../drude-model.md), $m\dot{\mathbf v}+m\gamma\mathbf v=-e\mathbf E$ gives

$$
\sigma(\omega)=\frac{ne^2}{m(\gamma-i\omega)},\qquad
\epsilon_r(\omega)=1-\frac{\omega_p^2}{\omega(\omega+i\gamma)},\qquad
\omega_p^2=\frac{ne^2}{m\epsilon_0},
$$

with a fixed positive ionic background and no additional bound-electron contribution in this simple model. The [plasma frequency](../../../../../plasma-frequency.md) marks the inertial electron-response scale. More elaborate band structure, interband transitions and nonlocal transport limit this scalar treatment.[Dielectric constant of a collisional plasma, equations (1201)–(1205): electron inertia, collisions and dielectric response](../../../../../electromagnetism-lecture-notes-by-richard-fitzpatrick.md)

In the collisionless nonmagnetic limit, the [dispersion relation](../../../../../dispersion-relation-split.md) is $\omega^2=\omega_p^2+c^2k^2$. For $\omega>\omega_p$,

$$
v_p=\frac\omega k=\frac{c}{\sqrt{1-\omega_p^2/\omega^2}}>c,\qquad
v_g=\frac{d\omega}{dk}=c\sqrt{1-\omega_p^2/\omega^2}<c.
$$

A crest can move faster than $c$ without carrying a new signal faster than [light](../../../../../light.md). Below cutoff the ideal wave is evanescent, with penetration [length](../../../../../length.md) $c/\sqrt{\omega_p^2-\omega^2}$; it does not propagate as an ordinary real-$k$ bulk wave. Evanescence in the lossless limit is not Joule dissipation. Nonzero collision rate gives a dissipative conductivity and smooths this ideal cutoff picture.

For a good conductor with approximately real $\sigma\gg\omega\epsilon$, the spatial branch becomes

$$
\boxed{k\simeq\frac{1+i}{\delta},\qquad\delta=\sqrt{\frac{2}{\mu\sigma\omega}}.}
$$

A field [amplitude](../../../../../wave-amplitude.md) falls as $e^{-z/\delta}$, while [intensity](../../../../../intensity-physics.md) falls as $e^{-2z/\delta}$. The [phase velocity](../../../../../phase-velocity.md) is $\omega\delta$ in this limit. Magnetic and electric [amplitudes](../../../../../wave-amplitude.md) are not related by the [vacuum](../../../../../vacuum.md) ratio: $Z_s=E/H=(1-i)\sqrt{\mu\omega/(2\sigma)}$ with the chosen time convention. Its positive real part is the surface resistance. The local mean heating is $\tfrac12\operatorname{Re}\sigma\,|E|^2$, consistent with electromagnetic [energy](../../../../../energy-split.md) flowing into the metal. [skin depth](../../../../../skin-depth.md) is an [amplitude](../../../../../wave-amplitude.md) [length](../../../../../length.md); interpreting it as an [intensity](../../../../../intensity-physics.md) [length](../../../../../length.md) gives a factor-of-two error.

A transmission-line mode propagates chiefly through the [dielectric](../../../../../dielectric.md) between conductors, even though finite metal conductivity causes loss at its boundaries. With per-length parameters $R',L',G',C'$, the [telegrapher's equations](../../../../../telegrapher-s-equations.md) give, for the same $e^{-i\omega t}$ convention,

$$
\frac{dV}{dz}=-(R'-i\omega L')I,\qquad
\frac{dI}{dz}=-(G'-i\omega C')V.
$$

Writing a forward wave as $e^{-\Gamma z}$, $\Gamma=\alpha-i\beta$, gives $\Gamma^2=(R'-i\omega L')(G'-i\omega C')$. In the low-loss regime $R'\ll\omega L'$ and $G'\ll\omega C'$, set $Z_0\simeq\sqrt{L'/C'}$ to obtain

$$
\boxed{\alpha\simeq\frac{R'}{2Z_0}+\frac{G'Z_0}{2},\qquad
\beta\simeq\omega\sqrt{L'C'}.}
$$

This [low-loss transmission-line attenuation](../../../../../low-loss-transmission-line-attenuation.md) separates series conductor loss from [dielectric](../../../../../dielectric.md) leakage loss. Average forward power falls as $e^{-2\alpha z}$. In the normal skin-effect regime, reduced conducting [area](../../../../../surface-area.md) makes the AC conductor resistance increase roughly as $\sqrt\omega$; [dielectric loss](../../../../../dielectric-loss.md) can supply a separate [frequency](../../../../../frequency.md) dependence. Reflection from a mismatched termination changes delivered power without being, by itself, dissipation in the line.[Chapter14, §§14.7–14.9: distributed losses, Ohmic waves and conductor-loss approximation](../../../../../electromagnetic-fields-and-energy-by-hermann-a-haus-and-james-r-melcher.md)

To test loss, compare several [lengths](../../../../../length.md) of otherwise identical line with matched terminations, calibrate connectors and incident/reflected power, and monitor [temperature](../../../../../temperature-split.md). Separate [amplitude](../../../../../wave-amplitude.md) attenuation from phase delay and from standing-wave minima. Bulk penetration, line attenuation and [dielectric](../../../../../dielectric.md) propagation [speed](../../../../../speed.md) are related electromagnetic quantities but describe different experimental geometries.

<a id="section-b/b7/image-conducting-wave-propagation"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1-conducting-waves.png)

**[Figure 1](#section-b/b7/image-conducting-wave-propagation). Conducting-wave propagation**. Chosen dispersion and decay models.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
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
