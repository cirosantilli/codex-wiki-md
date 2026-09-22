<h1 id="section-d/d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

A completely filled [valence band](../../../../../valence-band.md) carries no net current: its occupied crystal-momentum states have [velocities](../../../../../velocity.md) that cancel. Near a valence-band maximum, an almost full band is conveniently described by the few missing [electrons](../../../../../electron.md), or [electron holes](../../../../../electron-hole.md). Removing an [electron](../../../../../electron.md) of charge $-e_0$, with $e_0>0$, changes the charge relative to the filled band by $+e_0$. This is a [quasiparticle](../../../../../quasiparticle.md) description of electronic motion, not a mobile positive ion or a [Positron](../../../../../positron.md).

For an isotropic parabolic maximum, $\epsilon_v(\mathbf k)=E_v-\hbar^2k^2/(2m_h^*)$. Assign the missing-electron state momentum $\mathbf k_h=-\mathbf k_e$ and hole [energy](../../../../../energy-split.md)

$$
\epsilon_h(\mathbf k_h)=E_v-\epsilon_v(-\mathbf k_h)
=\frac{\hbar^2k_h^2}{2m_h^*}.
$$

It has positive [effective mass](../../../../../band-effective-mass.md) $m_h^*$. Its [velocity](../../../../../velocity.md) equals the [velocity](../../../../../velocity.md) of the missing [electron](../../../../../electron.md) state, and its positive-charge current replaces the negative of that state's electronic current. Semiclassical motion is thus $\hbar\dot{\mathbf k}_h=+e_0(\mathbf E+\mathbf v_h\times\mathbf B)$. With [momentum relaxation time](../../../../../momentum-relaxation-time.md) $\tau_h$, the low-field mobility is $\mu_h=e_0\tau_h/m_h^*$ and

$$
\boxed{\sigma_h=e_0p\mu_h=\frac{p e_0^2\tau_h}{m_h^*}.}
$$

If [electrons](../../../../../electron.md) also contribute, $\sigma=e_0(p\mu_h+n\mu_e)$: the two species' longitudinal conductivities add.

A [Hall bar](../../../../../hall-bar.md) separates carrier concentration from mobility. Apply [current density](../../../../../current-density.md) $j_x$, [magnetic field](../../../../../magnetic-field-split.md) $B_z$, and measure transverse [electric field](../../../../../electric-field-split.md) $E_y$. For one isotropic hole population, transverse [force](../../../../../force-split.md) balance gives $E_y=v_xB_z$, so

$$
\boxed{R_H=\frac{E_y}{j_xB_z}=\frac1{e_0p}>0,\qquad
p=\frac1{e_0R_H},\qquad \mu_h=\sigma R_H.}
$$

For thickness $t$, the Hall-voltage magnitude is $|V_H|=IB/(e_0pt)$. A longitudinal [four-terminal resistance measurement](../../../../../four-terminal-sensing.md) supplies $\sigma$ independently. Use [ohmic contacts](../../../../../ohmic-contact.md), known conducting thickness, controlled [temperature](../../../../../temperature-split.md) and low enough current to avoid self-heating. Reversing [magnetic field](../../../../../magnetic-field-split.md) removes even-in-field longitudinal offsets from contact misalignment; reversing current also helps reject thermoelectric offsets. These are central controls, rather than merely taking one transverse voltage reading.[Sample Geometry; Resistivity Measurements; Definitions for Hall Measurements; Hall Measurements and Hall Calculations](../../../../../resistivity-and-hall-measurements-by-national-institute-of-standards-and-technology.md)

The simple inference assumes one carrier type and a known [Hall scattering factor](../../../../../hall-scattering-factor.md). More generally $R_H=r_H/(e_0p)$, so $\sigma R_H$ measures [Hall mobility](../../../../../hall-mobility.md) rather than automatically the drift mobility. With two carrier populations at weak field,

$$
R_H=\frac{p\mu_h^2-n\mu_e^2}{e_0(p\mu_h+n\mu_e)^2}.
$$

Its sign alone need not identify the more numerous carrier. A Hall experiment also cannot determine $m_h^*$ and $\tau_h$ separately: their ratio sets mobility. [cyclotron resonance](../../../../../cyclotron-resonance.md) supplies an independent [mass](../../../../../mass.md) measurement by sweeping [frequency](../../../../../frequency.md) or [magnetic field](../../../../../magnetic-field-split.md) through $\omega=e_0B/m_c$ and detecting resonant absorption. The measured [cyclotron effective mass](../../../../../cyclotron-effective-mass.md) can depend on band anisotropy and need not equal every curvature [mass](../../../../../mass.md); the isotropic parabolic model identifies them. Its linewidth provides a scattering-time estimate only with a specified [damping](../../../../../damping.md) model.

<a id="section-d/d12/image-positive-curvature-hole-energy-a-hall-bar-measurement-and-an-acceptor-level-in-a-semiconductor"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2-holes.png)

**[Figure 5](#section-d/d12/image-positive-curvature-hole-energy-a-hall-bar-measurement-and-an-acceptor-level-in-a-semiconductor). Positive-curvature hole energy, a Hall-bar measurement, and an acceptor level in a semiconductor**.

[semiconductor doping](../../../../../semiconductor-doping.md) generates holes by adding [acceptor impurities](../../../../../acceptor-impurity.md). In [silicon](../../../../../silicon.md), a substitutional group-III atom such as [boron](../../../../../boron.md) provides one fewer valence [electron](../../../../../electron.md) than [silicon](../../../../../silicon.md). A shallow acceptor level lies slightly above the valence-band edge: accepting a valence [electron](../../../../../electron.md) makes the dopant negatively ionized and leaves a mobile hole in the [valence band](../../../../../valence-band.md). The impurity stays fixed in the lattice. [charge neutrality](../../../../../charge-neutrality.md) and the nondegenerate [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) mass-action law give

$$
p+N_D^+=n+N_A^-,\qquad np=n_i^2.
$$

For fully ionized, uncompensated acceptors in the extrinsic regime, $p\simeq N_A$ and $n\simeq n_i^2/N_A$; with fully ionized donor compensation, $p\simeq N_A-N_D$ while holes remain dominant. The [Fermi level](../../../../../fermi-level.md) moves towards the [valence band](../../../../../valence-band.md). At low [temperature](../../../../../temperature-split.md), [semiconductor carrier freeze-out](../../../../../semiconductor-carrier-freeze-out.md) suppresses mobile [electron holes](../../../../../electron-hole.md); at high [temperature](../../../../../temperature-split.md) intrinsic electron-hole generation can dominate. Increasing dopant density also changes scattering, so a conductivity increase alone cannot distinguish increased [carrier density](../../../../../carrier-density.md) from changed mobility. Temperature-dependent Hall and conductivity measurements separate these effects, subject to the carrier and scattering qualifications above.

## ↑ Ancestors (14)

1. [D12](../d12.md)
2. [Section D](../../section-d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
