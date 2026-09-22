<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

**Field equations.** In a homogeneous source-free nonmagnetic medium, $\mathbf D=\epsilon\varepsilon_0\mathbf E$ and $\mathbf B=\mu_0\mathbf H$. [Maxwell's equations](../../../../../maxwell-equations-split.md) become

$$
\boxed{\nabla\cdot\mathbf E=0,\quad\nabla\cdot\mathbf H=0,\quad
\nabla\times\mathbf E=-\mu_0\partial_t\mathbf H,\quad
\nabla\times\mathbf H=\epsilon\varepsilon_0\partial_t\mathbf E.}
$$

The first equation follows from $\nabla\cdot\mathbf D=0$ for spatially constant nonzero $\epsilon$. When the effective relative [permittivity](../../../../../permittivity-split.md) is negative below, its charge response is already included in $\mathbf D$; it must not also be counted as an extra free source.

**Amplitude relations and bulk dispersion.** Work with complex [phasors](../../../../../phasor.md) proportional to $e^{ikx-Kz-i\omega t}$. For $\mathbf H=(0,H_y,0)$, the [Ampere-Maxwell law](../../../../../ampere-s-circuital-law.md) gives

$$
(KH_y,0,ikH_y)=-i\omega\epsilon\varepsilon_0(E_x,0,E_z),
$$

so the amplitudes must obey

$$
\boxed{E_x=\frac{iK}{\omega\epsilon\varepsilon_0}H_y,\qquad
E_z=-\frac{k}{\omega\epsilon\varepsilon_0}H_y.}
$$

They are not arbitrary independent constants: the dispersion relation alone would not make arbitrary amplitudes satisfy the equations. These relations give $ikE_x-KE_z=0$, so the electric divergence vanishes; the magnetic divergence vanishes because there is no $y$ dependence. The only nonzero component of [Faraday's law of induction](../../../../../faraday-s-law-of-induction.md) is

$$
-KE_x-ikE_z=i\omega\mu_0H_y.
$$

Substitution then gives

$$
\boxed{k^2-K^2=\omega^2\epsilon\varepsilon_0\mu_0
=\frac{\omega^2\epsilon}{c^2}.}
$$

This proves that all four field equations hold for the specified [transverse magnetic polarization](../../../../../transverse-magnetic-polarization.md) when both the amplitude relations and the dispersion relation are imposed.

**Interface matching.** Let region 1 be vacuum above the interface, with $\epsilon_1=1$, $K=\beta_1>0$; region 2 has $\epsilon_2=\epsilon$, $K=\beta_2<0$. These signs make the [evanescent](../../../../../evanescent-wave.md) fields decay as $z\to\pm\infty$. In the absence of [free surface](../../../../../free-surface.md) current, tangential $H_y$ is continuous, giving a common interface amplitude. Tangential $E_x$ is also continuous, hence

$$
\frac{i\beta_1H_y}{\omega\varepsilon_0}
=\frac{i\beta_2H_y}{\omega\epsilon\varepsilon_0},
\qquad \boxed{\epsilon\beta_1=\beta_2.}
$$

Normal $D_z$ is continuous as well: both sides have $D_z=-kH_y/\omega$. This does not require $E_z$ itself to be continuous; the material can have polarization surface charge. The normal [magnetic field](../../../../../magnetic-field-split.md) is zero on both sides.

**Existence and surface dispersion.** The opposite signs of $\beta_1$ and $\beta_2$ require $\epsilon<0$. The two bulk equations are

$$
k^2-\beta_1^2=\frac{\omega^2}{c^2},\qquad
k^2-\beta_2^2=\frac{\omega^2\epsilon}{c^2}.
$$

Use $\beta_2^2=\epsilon^2\beta_1^2$ to eliminate the decay constants. For the nontrivial interface branch,

$$
\boxed{k^2=\frac{\omega^2}{c^2}\frac\epsilon{\epsilon+1},\qquad
\beta_1^2=-\frac{\omega^2/c^2}{\epsilon+1}.}
$$

A positive $\beta_1^2$ together with real propagating $k$ gives **$\epsilon<-1$**. A negative [permittivity](../../../../../permittivity-split.md) between $-1$ and zero is insufficient. This [lossless planar surface-plasmon dispersion](../../../../../lossless-planar-surface-plasmon-dispersion.md) describes a [surface plasmon polariton](../../../../../surface-plasmon-polariton.md); $\epsilon=1$ would instead be identical media and supplies no decaying bound mode.

**Frequency range and long wavelengths.** With $\epsilon=1-\omega_p^2/\omega^2$, the existence condition becomes

$$
\boxed{0<\omega<\frac{\omega_p}{\sqrt2}.}
$$

The upper value is a limiting [frequency](../../../../../frequency.md) approached as $k\to\infty$, not an attained maximum at finite $k$. Substitution into the dispersion relation gives

$$
k^2=\frac{\omega^2}{c^2}
\frac{\omega_p^2-\omega^2}{\omega_p^2-2\omega^2}.
$$

For $\omega\ll\omega_p$, choosing propagation in the positive $x$ direction,

$$
\boxed{k=\frac\omega c\left[1+\frac{\omega^2}{2\omega_p^2}
+O\left(\frac{\omega^4}{\omega_p^4}\right)\right]
\simeq\frac\omega c.}
$$

It approaches the vacuum light line from larger $k$. The vacuum decay constant is then $\beta_1\simeq\omega^2/(c\omega_p)$, so confinement becomes weak at low [frequency](../../../../../frequency.md). This calculation assumes the stated real, lossless effective [permittivity](../../../../../permittivity-split.md); dissipation would require complex propagation and decay constants.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
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
