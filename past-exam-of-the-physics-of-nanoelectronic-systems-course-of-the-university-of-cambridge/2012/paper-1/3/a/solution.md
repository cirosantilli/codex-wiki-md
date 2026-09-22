<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Exchange-split bands in a [ferromagnet](../../../../../ferromagnet.md) generally give a different spin-resolved [density of states](../../../../../density-of-states.md) for each [spin](../../../../../spin.md) branch, $D_\uparrow(E_F)$ and $D_\downarrow(E_F)$. If [spin](../../../../../spin.md) is approximately conserved across a multilayer, its two [spin](../../../../../spin.md) channels conduct in parallel. A [spin valve](../../../../../spin-valve.md) combines a comparatively fixed reference-layer [magnetization](../../../../../magnetization.md) with a soft free layer that rotates in a small applied field. Its readout depends on the relative angle, not simply the absolute [spin](../../../../../spin.md) population. Biasing the layers near a perpendicular alignment gives a useful [linear response](../../../../../linear-response-theory.md) instead of operating at the flat parallel/antiparallel extrema.

In [giant magnetoresistance](../../../../../giant-magnetoresistance.md), a metallic spacer separates ferromagnetic layers. Spin-dependent bulk and interface scattering make their channel resistances unequal. The density of available final $d$ states influences scattering of more mobile states; however, a large total [density of states](../../../../../density-of-states.md) does not by itself guarantee a large conductivity. The [scattering-weighted spin-channel asymmetry](../../../../../scattering-weighted-spin-channel-asymmetry.md) also involves velocity and scattering matrix elements. In the elementary identical-layer [two-current resistor model](../../../../../two-current-resistor-model.md), let each magnetic layer have resistances $a,b$ in the two [spin](../../../../../spin.md) channels and neglect spacer resistance. Parallel moments give channels $2a$ and $2b$, while antiparallel moments give $a+b$ in each channel. Therefore

$$
R_P=\frac{2ab}{a+b},\qquad R_{AP}=\frac{a+b}{2},\qquad
\boxed{\frac{R_{AP}-R_P}{R_P}=\frac{(a-b)^2}{4ab}.}
$$

One favorable [spin](../../../../../spin.md) channel traverses both aligned layers efficiently; reversal removes that common easy path. A conducting spacer adds resistance, and [spin](../../../../../spin.md) mixing weakens the separate-channel approximation. The channel asymmetry is material/interface dependent, so positive magnetoresistance is not a theorem for every pair of different [ferromagnets](../../../../../ferromagnet.md).[§§2.1–2.2, pp.947–948, spin-dependent scattering and two-current construction](../../../../../spin-dependent-transport-gmr-and-tmr-by-alain-schuhl-and-daniel-lacour.md)

In [tunnelling magnetoresistance](../../../../../tunnelling-magnetoresistance.md), the spacer is an ultrathin insulator and current flows across a [magnetic tunnel junction](../../../../../magnetic-tunnel-junction.md). In the simple spin-conserving [density-of-states tunnelling magnetoresistance model](../../../../../density-of-states-tunnelling-magnetoresistance-model.md), assume spin-independent matrix elements and low [voltage](../../../../../voltage.md). Available initial and final states give

$$
G_P=C(D_{1\uparrow}D_{2\uparrow}+D_{1\downarrow}D_{2\downarrow}),\qquad
G_{AP}=C(D_{1\uparrow}D_{2\downarrow}+D_{1\downarrow}D_{2\uparrow}).
$$

Writing $P_i=(D_{i\uparrow}-D_{i\downarrow})/(D_{i\uparrow}+D_{i\downarrow})$ and $G_0=CD_1D_2/2$, these become $G_P=G_0(1+P_1P_2)$ and $G_{AP}=G_0(1-P_1P_2)$. Thus

$$
\boxed{\mathrm{TMR}\equiv\frac{R_{AP}-R_P}{R_P}=\frac{2P_1P_2}{1-P_1P_2}.}
$$

The effective tunnelling polarization can depend on the barrier and orbital symmetry, not just a bulk density-of-states sketch. Crystalline MgO junctions exploit symmetry-selective transmission, so the elementary product model is not a quantitative universal formula for them.[2004 publisher abstract, crystalline MgO junctions and large room-temperature response](../../../../../giant-room-temperature-magnetoresistance-in-fe-mgo-fe-junctions-by-shinji-yuasa-and-others.md)

Both devices convert a free-layer rotation into an electrical change. A useful approximate GMR interpolation is $R(\theta)=R_P+\Delta R(1-\cos\theta)/2$; the elementary tunnelling model instead gives $G(\theta)=G_0(1+P_1P_2\cos\theta)$. The [spin-valve small-field sensitivity](../../../../../spin-valve-small-field-sensitivity.md) is a chain rule,

$$
\boxed{\frac{dR}{dB}=\frac{dR}{d\theta}\frac{d\theta}{dB},\qquad
\delta V=I_{\rm bias}\frac{dR}{dB}\,\delta B.}
$$

[magnetic anisotropy](../../../../../magnetic-anisotropy.md), biasing and pinning set the rotation susceptibility. Conducting-spacer GMR usually offers low resistance and supports current-in-plane or current-perpendicular geometries. [TMR](../../../../../tunnelling-magnetoresistance.md) uses perpendicular tunnelling, often offers a larger fractional signal and a larger resistance-area product, but demands uniform, stable barriers and has bias dependence and breakdown limits. Neither is automatically the better small-field sensor: heating, Johnson and low-frequency noise, domain switching, hysteresis and stability set the detectable field. Reverse sweep direction, vary current and [temperature](../../../../../temperature-split.md), and independently test reference-layer pinning to distinguish a reproducible magnetic signal from drift or heating.

<a id="3/a/image-spin-dependent-sensor-response"></a>
![](../../../../../past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2012/paper-1-spin-sensors.png)

**[Figure 5](#3/a/image-spin-dependent-sensor-response). Spin-dependent sensor response**.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics of Nanoelectronic Systems course of the University of Cambridge](../../../../split.md)
6. [Physics of Nanoelectronic Systems course of the University of Cambridge](../../../../../physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
