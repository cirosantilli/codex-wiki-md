<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

TODO: biomolecular [force](../../../../../force-split.md) assays are user-deferred. The following notes cover the generic physical apparatus, calibrated dielectric handles and synthetic attachments only.

In [optical tweezers](../../../../../optical-tweezers.md), a tightly focused [laser](../../../../../laser-split.md) produces a restoring gradient [force](../../../../../force-split.md) on a suitable transparent bead. Scattering also transfers [momentum](../../../../../momentum-split.md) along propagation, so a stable three-dimensional trap needs axial as well as lateral restoration. An objective with high [numerical aperture](../../../../../numerical-aperture.md), correctly filled entrance pupil, controlled beam [polarization](../../../../../polarization-waves.md) and low-aberration sample chamber are practical design elements. Collect transmitted/scattered light with a condenser and measure bead [displacement](../../../../../displacement.md) with calibrated imaging or back-focal-plane photodetection. A steerable beam or translation stage sets relative positions; the [force](../../../../../force-split.md) signal comes from bead [displacement](../../../../../displacement.md), not commanded stage [displacement](../../../../../displacement.md) alone.

Near a stable operating point, use a [harmonic optical trap](../../../../../harmonic-optical-trap.md) with $U(x)=kx^2/2$. For a slowly changing external [force](../../../../../force-split.md), $F_{\rm ext}=k\langle x\rangle$ in that coordinate; the optical [restoring force](../../../../../restoring-force.md) is $-kx$. Calibrate each axis and the range over which its response is linear. Detector sensitivity must also be known: write $x=\beta(s-s_0)$, with measured detector voltage $s$, offset $s_0$ and position sensitivity $\beta$ in $\mathrm{m/V}$. A [spring constant](../../../../../spring-constant.md) in arbitrary detector units is not a [force](../../../../../force-split.md) calibration.

Three complementary physical calibrations are useful. At [thermal equilibrium](../../../../../thermal-equilibrium-split.md) the [equipartition theorem](../../../../../equipartition-theorem.md) gives

$$
\boxed{k=\frac{k_BT}{\langle(x-\langle x\rangle)^2\rangle}.}
$$

This needs an independently calibrated position scale and a [variance](../../../../../variance-split.md) corrected for drift, detector noise and exposure averaging. In an overdamped Newtonian medium, the [optical trap Langevin calibration](../../../../../optical-trap-langevin-calibration.md) obeys

$$
\zeta\dot x=-kx+\xi(t),\qquad
\langle\xi(t)\xi(t')\rangle=2k_BT\zeta\delta(t-t').
$$

Using a one-sided position [power spectral density](../../../../../power-spectral-density.md) per hertz,

$$
\boxed{S_x(f)=\frac{k_BT}{\pi^2\zeta(f^2+f_c^2)},\qquad
f_c=\frac{k}{2\pi\zeta},\qquad\int_0^\infty S_x(f)df=\frac{k_BT}{k}.}
$$

The corner [frequency](../../../../../frequency.md) and spectral amplitude test both relaxation and fluctuation size. If drag is known, $k=2\pi\zeta f_c$. The isolated-sphere value $\zeta=6\pi\eta a$ must be corrected near boundaries; otherwise measured height dependence can be mistaken for a changed trap stiffness. An independent steady [optical trap drag calibration](../../../../../optical-trap-drag-calibration.md) moves fluid past the trapped sphere: $k\langle x\rangle=\zeta u$. Use small positive and negative speeds to verify slope, offset and [force](../../../../../force-split.md) range.

One can also determine position sensitivity without assuming the bulk drag. In a low-frequency [sinusoidal-stage optical trap calibration](../../../../../sinusoidal-stage-optical-trap-calibration.md), let the known local fluid [velocity](../../../../../velocity.md) amplitude be $u_0$ at drive [angular frequency](../../../../../angular-frequency.md) $\Omega$. The coherent bead [displacement](../../../../../displacement.md) amplitude is

$$
A_x=\frac{\zeta u_0}{\sqrt{k^2+\Omega^2\zeta^2}}
=\frac{u_0}{\sqrt{(2\pi f_c)^2+\Omega^2}}.
$$

If the corresponding detector amplitude is $A_s$, then

$$
\boxed{\beta=\frac{u_0}{A_s\sqrt{(2\pi f_c)^2+\Omega^2}}.}
$$

After removing the coherent drive line from the thermal record, combine this sensitivity with [equipartition theorem](../../../../../equipartition-theorem.md) to recover $k$, and then infer $\zeta$ from $f_c$. A published calibration combines thermal spectra and stage-driven motion without taking bead drag as an input.[2006 author preprint, abstract: combined thermal/stage calibration and drag-independent sensitivity](../../../../../calibration-of-optical-tweezers-with-positional-detection-in-the-back-focal-plane-by-simon-f-tolic-norrelykke-and-others.md)

Controls determine whether these formulas measure the apparatus rather than its noise. Record blocked-light offsets and independent fixed-bead noise; calibrate [length](../../../../../length.md) with known motion; keep sampling and electronics bandwidth adequate around $f_c$; and include exposure filtering and [aliasing](../../../../../aliasing.md) in a spectral fit. [motion blur](../../../../../motion-blur.md) reduces measured [variance](../../../../../variance-split.md) and therefore makes naive [equipartition theorem](../../../../../equipartition-theorem.md) overestimate stiffness; additive position noise has the opposite bias. Changing exposure time provides a direct diagnostic.[§II, equations (12)–(18): variance reduction, temporal filter and aliased spectrum](../../../../../the-effect-of-integration-time-on-fluctuation-measurements-calibrating-an-optical-trap-in-the-presence-of-motion-blur-by-wesley-p-wong-and-others.md) Check [temperature](../../../../../temperature-split.md) and [laser](../../../../../laser-split.md) heating, wall separation, bead size and [refractive index](../../../../../refractive-index.md), alignment and power stability. Repeat after changing power or optical geometry and compare thermal, spectral and drag estimates. For a synthetic [force](../../../../../force-split.md) handle, also measure the attachment's compliance and geometry so that bead motion is not automatically identified with its extension.

<a id="3/a/image-optical-trap-calibration"></a>
![](../../../../../past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2012/paper-1-trap-calibration.png)

**[Figure 2](#3/a/image-optical-trap-calibration). Optical trap calibration**.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the soft matter and biological physics course of the University of Cambridge](../../../../split.md)
6. [Soft Matter and Biological Physics course of the University of Cambridge](../../../../../soft-matter-and-biological-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
