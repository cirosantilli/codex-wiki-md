<h1 id="section-b/b3/gain-and-effective-collecting-area">Gain and effective collecting area</h1>

↑ **Parent:** [Solution](solution.md)

[Antenna gain](../../../../antenna-gain.md) in direction $(\theta,\phi)$ compares the far-field [power](../../../../power.md) per solid angle with an isotropic radiator using the same accepted input [power](../../../../power.md):

$$
G(\theta,\phi)=\frac{4\pi}{P_{\rm in}}\frac{dP}{d\Omega}.
$$

It includes radiation efficiency; for the lossless dipole $P_{\rm in}=P_{\rm rad}$. The [antenna effective area](../../../../antenna-effective-area.md) is defined for incidence from a specified direction with matched polarization and conjugate impedance matching:

$$
P_{\rm available}=A_{\rm eff}(\theta,\phi)S_{\rm inc}.
$$

Its units are square metres and it need not equal the physical metal area.

For ordinary reciprocal antennas, [electromagnetic reciprocity](../../../../reciprocity-electromagnetism.md) makes the coupling between two matched ports the same when transmitter and receiver are exchanged. Free-space transfer in one direction is proportional to $G_1A_2$, while the reverse transfer is proportional to $G_2A_1$. Thus $A/G$ must be a universal factor at that [wavelength](../../../../wavelength.md), independent of antenna or direction. The supplied relation fixes it as

$$
\boxed{A_{\rm eff}(\theta,\phi)=\frac{\lambda^2}{4\pi}G(\theta,\phi).}
$$

Equivalently, thermal detailed balance prevents an angular receiving pattern from collecting more radiation than its reciprocal emitting pattern would return in equilibrium. Reciprocity and the specified matching are the assumptions behind this statement; it is not a general theorem for active nonreciprocal devices.

## ↑ Ancestors (14)

1. [Solution](solution.md)
2. [B3](../b3.md)
3. [Section B](../../section-b.md)
4. [2018](../../../2018-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
