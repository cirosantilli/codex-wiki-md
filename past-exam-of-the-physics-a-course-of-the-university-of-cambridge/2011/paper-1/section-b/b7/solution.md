<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

A [wave packet](../../../../../wave-packet.md) is a localized [superposition](../../../../../superposition-principle.md) of nearby [wavenumbers](../../../../../wavenumber.md). Its rapid carrier crests have [phase velocity](../../../../../phase-velocity.md) $v_p=\omega/k$; the slowly varying envelope translates at the [group velocity](../../../../../group-velocity.md). Dispersion means that $\omega(k)$ is not simply a constant times $k$, so different carrier components have different [phase velocities](../../../../../phase-velocity.md). Expand around $k_0$:

$$
u(x,t)=\operatorname{Re}\!\int A(k)e^{i[kx-\omega(k)t]}\,dk
\simeq\operatorname{Re}\!\left\{e^{i(k_0x-\omega_0t)}\int A(k_0+\kappa)e^{i\kappa[x-\omega'(k_0)t]}\,d\kappa\right\}.
$$

The integral is an envelope depending on $x-\omega'(k_0)t$, so **$v_g=d\omega/dk$** at the central [frequency](../../../../../frequency.md). Neglected curvature causes packet spreading. For a [deep-water gravity wave](../../../../../deep-water-gravity-wave.md), $\omega=\sqrt{gk}$, hence $v_p=\sqrt{g/k}$ and

$$
\boxed{v_g=\tfrac12\sqrt{g/k}=v_p/2=\frac{gT}{4\pi}.}
$$

For [crest crossings through a dispersive wave packet](../../../../../crest-crossings-through-a-dispersive-wave-packet.md), an instantaneous group containing six crests has length approximately $L=6\lambda$. A stationary ship takes $L/v_g$ to encounter the group; its crest-arrival [frequency](../../../../../frequency.md) is $v_p/\lambda$. Consequently

$$
\boxed{N=\frac{v_p}{\lambda}\frac L{v_g}=12.}
$$

In the envelope frame the ship moves backwards at $v_g$ while crests move forwards at $v_p-v_g=v_g$. Their relative speed is $2v_g$, explaining why counting a snapshot and counting crossings differ.

<a id="section-b/b7/image-six-crests-in-a-packet-and-twelve-ship-crossings"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1-wave-group.png)

**[Figure 3](#section-b/b7/image-six-crests-in-a-packet-and-twelve-ship-crossings). Six crests in a packet and twelve ship crossings**. Original narrow-band deep-water model. The right panel is in the envelope frame; only crest trajectories intersecting the ship while it is inside the packet are drawn.

To estimate [deep-water swell distance from period-dependent arrival times](../../../../../deep-water-swell-distance-from-period-dependent-arrival-times.md), assume a localized storm emits both periods at the same time and place, propagation is in deep water, and currents and refraction can be neglected. If its distance is $D$, the arrival lag obeys

$$
86400=D\left(\frac1{v_g(15\,\mathrm s)}-\frac1{v_g(20\,\mathrm s)}\right)
=\frac{4\pi D}{g}\left(\frac1{15}-\frac1{20}\right).
$$

With $g=9.81\,\mathrm{m\,s^{-2}}$, **$D=15g(86400)/\pi\simeq4.05\times10^6\,\mathrm m$**, about **4050 km**. The corresponding travel times are three and four days. A moving or long-lived storm with frequency-dependent emission times would invalidate the unique distance inference.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
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
