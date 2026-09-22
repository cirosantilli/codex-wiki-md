<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [X-ray](../../../../x-ray.md) [wavelength](../../../../wavelength.md) is $\lambda=hc/E=1.54980\times10^{-10}\,\mathrm m$. Write the amplitude of one conventional [unit cell](../../../../unit-cell.md) as the [face-centred cubic selection rule](../../../../face-centred-cubic-selection-rule.md) times the two-atom [atomic basis](../../../../atomic-basis-of-a-crystal.md) amplitude:

$$
F_{hkl}=\left[1+e^{i\pi(k+l)}+e^{i\pi(h+l)}+e^{i\pi(h+k)}\right]
\left[f_{\mathrm{Ga}}+f_{\mathrm{As}}e^{i\pi(h+k+l)/2}\right].
$$

The first bracket is four when the indices have equal parity and zero otherwise. Among the allowed [Bragg reflections](../../../../bragg-reflection.md), the [zinc blende structure factor](../../../../zinc-blende-structure-factor.md) therefore gives

$$
|F_{hkl}|^2=16\begin{cases}
f_{\mathrm{Ga}}^2+f_{\mathrm{As}}^2,&h,k,l\text{ odd},\\
(f_{\mathrm{Ga}}+f_{\mathrm{As}})^2,&h+k+l\equiv0\pmod4,\\
(f_{\mathrm{Ga}}-f_{\mathrm{As}})^2,&h+k+l\equiv2\pmod4.
\end{cases}
$$

Here the [atomic scattering factors](../../../../atomic-scattering-factor.md) are taken as real. For the requested rough estimate set $f_{\mathrm{Ga}}\simeq31$ and $f_{\mathrm{As}}\simeq33$. The weak difference reflections remain allowed: unequal species do not have the extra exact extinction of the equal-species diamond limit.

The first six allowed values of $h^2+k^2+l^2$ are $3,4,8,11,12,16$. [Bragg's law](../../../../bragg-s-law.md) gives the measured scattering angle $2\theta=2\sin^{-1}(\lambda\sqrt{h^2+k^2+l^2}/2a)$. For [powder diffraction](../../../../powder-diffraction.md), multiply the squared amplitude by the [powder diffraction multiplicity](../../../../powder-diffraction-multiplicity.md) $m_{hkl}$. The last two columns use $I_{111}=100$:

$$
\begin{array}{c|r|r|r|r|r}
hkl&2\theta\ ({}^\circ)&m_{hkl}&|F|^2&I\propto m|F|^2&I\propto m|F|^2LP\\\hline
111&27.4693&8&32800&100&100\\
200&31.8234&6&64&0.1463&0.1068\\
220&45.6248&12&65536&299.707&98.684\\
311&54.0830&24&32800&300&67.110\\
222&56.6994&8&64&0.1951&0.03921\\
400&66.5025&6&65536&149.854&21.165
\end{array}
$$

The first intensity column is the geometry-independent multiplicity-and-structure estimate. The second additionally assumes an unpolarized beam and a common symmetric powder-diffractometer geometry, with [Lorentz-polarization factor](../../../../lorentz-polarization-factor.md)

$$
LP(\theta)\propto\frac{1+\cos^2(2\theta)}{\sin^2\theta\cos\theta}.
$$

An overall constant cancels in either normalization. A particular measured intensity set is not fixed by the atomic numbers alone: actual [atomic scattering factors](../../../../atomic-scattering-factor.md) decrease with momentum transfer, anomalous scattering and absorption can matter, and the instrument geometry and [polarization](../../../../polarization-waves.md) determine angular corrections. The two columns state the approximation rather than asserting identical peak heights for all instruments.[Section 4, equation 5 and sections 4.1–4.2: multiplicity, structure amplitude and geometry-dependent polarization and Lorentz corrections](../../../../quantitative-powder-diffraction-using-a-2-plus-3-surface-diffractometer-and-an-area-detector-by-giuseppe-abbondanza-and-others.md)

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
