<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

For fixed, magnetically linear geometry, [self-inductance](../../../../../self-inductance.md) relates a coil's own [magnetic flux linkage](../../../../../magnetic-flux-linkage.md) to its [electric current](../../../../../electric-current.md), $\Lambda_i=L_iI_i$. [mutual inductance](../../../../../mutual-inductance.md) relates the linkage in one coil to the current in the other, $\Lambda_{21}=MI_1$. These coefficients enter the induced [electromotive forces](../../../../../electromotive-force.md) through $\mathcal E_i=-d\Lambda_i/dt$; reversing a chosen winding orientation reverses the sign assigned to $M$.

In the ideal confined-field [toroid](../../../../../toroid.md), a circular [magnetostatic Ampère law](../../../../../magnetostatic-ampere-law.md) contour encloses $N_1I$, so

$$
\boxed{H_\phi(r)=\frac{N_1I}{2\pi r}\quad(a<r<b).}
$$

Write $w=b-a$ for the height of the square cross-section. The [inductance of a rectangular-section toroid](../../../../../inductance-of-a-rectangular-section-toroid.md) follows by integrating the [magnetic flux density](../../../../../magnetic-field-split.md) over that cross-section; it cannot be replaced by its value at an arbitrary mean [radius](../../../../../radius.md):

$$
\Phi=w\int_a^b\mu_0\mu_rH_\phi(r)\,dr
=\frac{\mu_0\mu_rN_1Iw}{2\pi}\ln\frac ba.
$$

Consequently, for winding normals chosen consistently,

$$
\boxed{L_i=\frac{\mu_0\mu_rN_i^2(b-a)}{2\pi}\ln\frac ba,\qquad
M_0=\frac{\mu_0\mu_rN_1N_2(b-a)}{2\pi}\ln\frac ba=\sqrt{L_1L_2}.}
$$

The equality means complete shared [magnetic flux linkage](../../../../../magnetic-flux-linkage.md); with leakage one instead has $|M|<\sqrt{L_1L_2}$.

For the crack, use the [radial-path approximation for a cracked toroid](../../../../../radial-path-approximation-for-a-cracked-toroid.md), with an air [length](../../../../../length.md) $d$ on each path and core [length](../../../../../length.md) $2\pi r-d$. Continuity of the normal [magnetic flux density](../../../../../magnetic-field-split.md) at a crack face gives $H_g=\mu_rH_c$. Hence

$$
N_1I=\frac{B(r)}{\mu_0\mu_r}(2\pi r-d)+\frac{B(r)}{\mu_0}d,
\qquad
B(r)\simeq\frac{\mu_0\mu_rN_1I}{2\pi r+(\mu_r-1)d}.
$$

Integrating the radial paths yields

$$
M_d\simeq\frac{\mu_0\mu_rN_1N_2w}{2\pi}
\ln\frac{b+q}{a+q},\qquad q=\frac{(\mu_r-1)d}{2\pi},
\qquad
\boxed{\frac{M_d-M_0}{M_0}\simeq
\frac{\ln[(b+q)/(a+q)]}{\ln(b/a)}-1=-0.529.}
$$

Here $q=1.5915\,\mathrm{cm}$ and $M_d/M_0=0.47079$: **about a 53% reduction**. The small ratio $d/a$ does not justify expanding in $\mu_rd/a$, which is about ten. The crack's low [magnetic permeability](../../../../../permeability-electromagnetism.md) gives appreciable [magnetic reluctance](../../../../../magnetic-reluctance.md). This is an estimate within a confined-flux model; actual redistribution near the slit is outside its accuracy. Narrow-gap circuit models assume small gap width relative to transverse dimensions and approximately directed flux.[§9.7, Example 9.7.1 and the paragraph after it: air-gap circuit approximation and need for a more general field solution](../../../../../electromagnetic-fields-and-energy-by-hermann-a-haus-and-james-r-melcher/magnetic-circuits.md)

For the intact ring, ideal poloidal winding currents and the no-leakage boundary condition admit $\mathbf H=N_1I\widehat{\boldsymbol\phi}/(2\pi r)$ with zero radial and vertical components. It is curl-free inside the current-free core, divergence-free for uniform [magnetic permeability](../../../../../permeability-electromagnetism.md), tangent to the core boundary, and has the required [circulation](../../../../../circulation-physics.md); [uniqueness of the Neumann problem](../../../../../uniqueness-of-the-neumann-problem.md) removes an additional homogeneous scalar-potential field. This explains zero non-azimuthal components in the stipulated intact-ring idealization. A literal slit breaks that rotational [symmetry](../../../../../symmetry-physics.md), so **zero transverse components everywhere is not exact for the cracked ring**: [magnetic fringing](../../../../../magnetic-fringing.md) and flux redistribution occur. In fact, extending the approximate $B(r)\propto1/(r+q)$ unchanged around a current-free core would give $[\nabla\times\mathbf H]_z\ne0$. Thus that radial-path calculation and a claim of exact purely azimuthal field in the cracked geometry cannot both be exact. The numerical answer above retains the intended circuit approximation while making its limitation explicit.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
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
