<h1 id="b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

Here $\mathbf H$ is [magnetic field intensity](../../../../magnetic-field-intensity.md), $\mathbf J$ free [electric current](../../../../electric-current.md) [density](../../../../density.md), and $\mathbf D$ electric displacement. In vacuum, $\mathbf B=\mu_0\mathbf H$ and $\mathbf D=\epsilon_0\mathbf E$. Integrating the equation gives [Ampère's circuital law](../../../../ampere-s-circuital-law.md) with [displacement current](../../../../displacement-current.md); in a [steady state](../../../../steady-state.md) the displacement term vanishes.

Take $z$ upward and define $V=\phi_{\rm upper}-\phi_{\rm lower}=V_0\sin\omega t$. Neglect fringing and use the low-frequency thin-capacitor approximation. Then

$$
\boxed{\mathbf E=E_z(t)\hat{\mathbf z},\qquad
E_z=-\frac{V_0}{L}\sin\omega t,\qquad E_r=E_\phi=0.}
$$

Inside the gap, a circular Ampère loop encloses only [displacement current](../../../../displacement-current.md):

$$
2\pi rH_\phi=\epsilon_0\pi r^2\dot E_z,
\qquad
\boxed{\mathbf H=\frac{\epsilon_0r}{2}\dot E_z\,\hat{\boldsymbol\phi}
=-\frac{\epsilon_0r\omega V_0}{2L}\cos\omega t\,\hat{\boldsymbol\phi}.}
$$

Because $\hat{\mathbf z}\times\hat{\boldsymbol\phi}=-\hat{\mathbf r}$, the [Poynting vector](../../../../poynting-vector.md) is

$$
\boxed{\mathbf S=-\frac{\epsilon_0r}{2}E_z\dot E_z\,\hat{\mathbf r}.}
$$

It points inward while the electrical [energy](../../../../energy-split.md) is increasing and outward while it decreases. The net [power](../../../../power.md) entering the curved side is

$$
-2\pi aL S_r(a)=\epsilon_0\pi a^2L E_z\dot E_z
=\frac d{dt}\left(\frac{\epsilon_0\pi a^2L}{2}E_z^2\right)
=\dot U_E.
$$

This is the leading quasistatic [energy](../../../../energy-split.md) balance. The time-averaged field energies are

$$
\overline U_E=\frac{\epsilon_0\pi a^2V_0^2}{4L},\qquad
\overline U_B=\frac{\mu_0\epsilon_0^2\omega^2\pi a^4V_0^2}{32L},
\qquad
\boxed{\frac{\overline U_B}{\overline U_E}=\frac18\left(\frac{\omega a}{c}\right)^2.}
$$

For the [axisymmetric high-frequency capacitor field](../../../../axisymmetric-high-frequency-capacitor-field.md) when $\omega a/c$ is not small, induction and radial propagation prevent a spatially uniform $E_z$. In an ideal axially uniform axisymmetric interior model, Faraday's and Ampère's equations give

$$
\frac1r\frac d{dr}\left(r\frac{dE_z}{dr}\right)+\frac{\omega^2}{c^2}E_z=0.
$$

The solution regular at the axis and normalized to the central [voltage](../../../../voltage.md) is approximately

$$
\boxed{E_z(r,t)=-\frac{V_0}{L}J_0(\omega r/c)\sin\omega t.}
$$

At $\omega=\pi c/a$, the radial profile is $J_0(\pi r/a)$: its first zero is at $r\simeq0.765a$, and the edge has opposite [phase](../../../../phase-waves.md), $J_0(\pi)\simeq-0.304$. This is an illustrative thin-disc interior profile; the exact driven high-frequency field also depends on the feed and edge/radiation [boundary conditions](../../../../boundary-condition.md). Continuing the uniform quasistatic field would be inconsistent.

<a id="b8/image-original-ideal-axisymmetric-capacitor-field-profiles-comparing-the-uniform-quasistatic-limit-with-the-bessel-radial-profile-at-angular-frequency-pi-times-c-over-a"></a>
![](../../../../past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1-gpp2014-capacitor-profile.png)

**[Figure 4](#b8/image-original-ideal-axisymmetric-capacitor-field-profiles-comparing-the-uniform-quasistatic-limit-with-the-bessel-radial-profile-at-angular-frequency-pi-times-c-over-a). Original ideal axisymmetric capacitor field profiles, comparing the uniform quasistatic limit with the Bessel radial profile at angular frequency pi times c over a**.

## ↑ Ancestors (12)

1. [B8](../b8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
