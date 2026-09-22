# Gouy balance

↑ **Parent:** [Magnetic susceptibility](magnetic-susceptibility.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gouy_balance)

A [Gouy balance](gouy-balance.md) detects the [force](force-split.md) exerted by a nonuniform [magnetic field](magnetic-field-split.md) on a sample of uniform cross-section extending between high- and low-field regions. TeachSpin's implementation reverses the usual arrangement: a rare-earth permanent-magnet assembly sits on a one-pan electronic balance, while a separate holder brings the sample into the field. The magnet's apparent mass change measures the opposite of the sample's vertical [force](force-split.md), by [Newton's third law](newton-s-third-law.md). The described pole faces have diameter $25\,\mathrm{mm}$ and separation $15\,\mathrm{mm}$; samples occupy cuvettes of cross-section $(10\,\mathrm{mm})^2$ and height about $32\,\mathrm{mm}$. [TeachSpin, Foundational Magnetic Susceptibility, Instrument: The Gouy Method and “Weighing the magnet” method; Specifications: magnet and sample dimensions](foundational-magnetic-susceptibility-by-teachspin.md)

The same balance calibrates [magnetic flux density](magnetic-field-split.md) by measuring the reaction [force](force-split.md) on the magnet when a wire of known horizontal length $L$ carries known [electric current](electric-current.md) $i$ perpendicular to the field: $|F_z|=iLB_0$. The manufacturer describes water being repelled by the high-field region, identifying negative [magnetic susceptibility](magnetic-susceptibility.md). This observed sign supplies a qualitative test, not a measured [Curie's law](curie-s-law.md) curve. [TeachSpin, Foundational Magnetic Susceptibility, Instrument: Absolute calibration method and Diamagnetism](foundational-magnetic-susceptibility-by-teachspin.md)

For weak reversible linear response, a uniform sample displacing a weakly magnetic surrounding medium has, to leading order, downward [force](force-split.md)

$$
F_\downarrow\simeq\frac{A(\chi_v-\chi_{\rm medium})}{2\mu_0}
\left(B_{0,\rm bottom}^2-B_{0,\rm top}^2\right).
$$

This follows by integrating the induced-dipole force density $(\chi_v-\chi_{\rm medium})\partial_z(B_0^2)/(2\mu_0)$ along a downward coordinate. $A$ is the cross-sectional [area](surface-area.md), and the two $B_0$ values are applied [magnetic flux densities](magnetic-field-split.md). The [force](force-split.md) depends on the endpoint fields; the entire field-gradient profile need not be measured under these assumptions. In the reversed apparatus, $F_\downarrow=-g\Delta m_{\rm magnet}$ after subtracting the holder background, where $g$ is [gravitational acceleration](gravitational-acceleration.md). This sign must be reversed before inferring [volume magnetic susceptibility](volume-magnetic-susceptibility.md).

Useful controls are an empty-holder reading at the same position, a distant-sample baseline, repeated wire-current reversals during field calibration, and stable [temperature](temperature-split.md). They separate holder response, balance drift, force offsets, and thermal changes; these are proposed checks for the stated inference. Finite endpoint fields, nonuniform cross-section, uneven powder packing, stray forces and a [demagnetizing field](demagnetizing-field.md) limit the simple formula. If [magnetization](magnetization.md) is nonlinear, the weak-response force involves $A\int_{B_{0,\rm top}}^{B_{0,\rm bottom}}M(B_0)\,dB_0$ instead of a constant-$\chi_v$ endpoint square. A balance reading then measures an integrated response, not directly the local [differential magnetic susceptibility](differential-magnetic-susceptibility.md).

## ↑ Ancestors (5)

1. [Magnetic susceptibility](magnetic-susceptibility.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gouy balance](gouy-balance.md)
- [Magnetic susceptibility](magnetic-susceptibility.md)
