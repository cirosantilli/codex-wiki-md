<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Hall-plateau voltmeter calibration](../../../../hall-plateau-voltmeter-calibration.md) is obtained as follows. Let $D_p$ be a plateau height in displayed units after any voltage offset is removed, with identified integer plateau index $p$. The true [Hall voltage](../../../../hall-voltage.md) is $I_xR_K/p$, so the [calibration](../../../../calibration-differential-geometry.md) factor would be

$$
\boxed{\lambda=\frac{I_xR_K}{pD_p}
=\frac{3.8719\times10^{-4}}{pD_p}\,\mathrm{V/(displayed\ unit)}.}
$$

The nominal current is $15\,\mathrm{nA}$. If several plateau heights are available, their inverse-integer ratios help identify indices and a fit of $D_p$ against $1/p$ can separate a constant offset from the gain. Reversing [magnetic field](../../../../magnetic-field-split.md) and antisymmetrizing the voltage also removes an even offset. A unique absolute index should not be asserted solely from an unspecified sequence of steps.

For an established exact integer $p$ and independent current and height errors,

$$
\boxed{\left(\frac{\delta\lambda}{\lambda}\right)^2
=\left(\frac{0.3}{15}\right)^2+\left(\frac{\delta D_p}{D_p}\right)^2.}
$$

The current alone contributes $2\%$ relative uncertainty; it is a common [calibration](../../../../calibration-differential-geometry.md) uncertainty and does not average away by fitting more plateaux. Voltage-offset uncertainty and deviations from quantization must also be included where relevant. The $25\pm2\,\mu\mathrm m$ width cancels because the Hall _voltage_ divided by current is a sheet Hall resistance; it would enter the transverse [electric field](../../../../electric-field-split.md), not this [calibration](../../../../calibration-differential-geometry.md).

**TODO — missing source data:** the held PDF's last-page stream refers to an absent `/Im6` graphic, and its recovery log reports an unknown XObject. The supplied TeX records the same source gap. No plateau heights, labels or axis values survive, so neither a numerical $D_p$ nor a unique $p$ can be read. The numerical voltmeter [calibration](../../../../calibration-differential-geometry.md) and its complete graph-reading error cannot be supplied without that graph; the formula and known $2\%$ current contribution above are determined.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
