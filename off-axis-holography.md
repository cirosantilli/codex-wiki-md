# Off-axis holography

↑ **Parent:** [Holography](holography.md)

[Off-axis holography](off-axis-holography.md) tilts the [holographic reference wave](holographic-reference-wave.md) relative to the [holographic object wave](holographic-object-wave.md). Its [interference fringes](interference-fringe.md) acquire a carrier [spatial frequency](spatial-frequency.md); the two cross terms occupy different [spatial frequency](spatial-frequency.md) regions when the carrier is sufficiently large compared with the object's [signal bandwidth](signal-bandwidth.md). This permits filtering a single image term.

Gabor's lecture credits [Emmett Leith](emmett-leith.md) and [Juris Upatnieks](juris-upatnieks.md) with the later skew-reference method using helium–neon [laser](laser-split.md) illumination, separating reconstructed images angularly.[Gabor, Nobel lecture, Fig. 8 and surrounding account of the 1962–1963 laser work](holography-1948-1971-by-dennis-gabor.md)

For an original periodic calculation, let $x$ run over a unit-length [interval](interval-mathematics.md) and choose

$$
O(x)=0.2e^{2\pi i3x}+0.1e^{-2\pi i5x},\qquad R(x)=e^{2\pi i20x}.
$$

All [spatial frequencies](spatial-frequency.md) here are cycles per unit length; the data are a chosen field at the recording plane, not measurements or a physical object profile. Direct expansion gives

$$
I(x)=1.05+0.04\cos(2\pi8x)+0.4\cos(2\pi17x)+0.2\cos(2\pi25x).
$$

Consequently its [Fourier series](fourier-series-split.md) coefficients are $1.05$ at zero, $0.02$ at $\pm8$, $0.2$ at $\pm17$ and $0.1$ at $\pm25$. The $R^*O$ component lies at $-17,-25$; the $RO^*$ component lies at $17,25$; the background lies at $0,\pm8$. Filtering the negative-frequency cross term and multiplying by $R$ recovers $O$, including its relative [wave phase](phase-waves.md).

<a id="image-original-periodic-off-axis-holography-calculation-separated-cross-terms-and-recovered-complex-amplitude"></a>
![](holography-off-axis-cross-term-separation.png)

**[Figure 20](#image-original-periodic-off-axis-holography-calculation-separated-cross-terms-and-recovered-complex-amplitude). Original periodic off-axis holography calculation: separated cross terms and recovered complex amplitude**.

The figure samples $N=1024$ equally spaced positions with the endpoint excluded, computes a normalized [discrete Fourier transform](discrete-fourier-transform-split.md) using a [Fast Fourier transform](fast-fourier-transform.md), retains bins $-30\leq m\leq-12$, then applies the [inverse discrete Fourier transform](inverse-discrete-fourier-transform.md) and multiplies by $R$. The recovered real and imaginary parts coincide with the chosen $O$ to numerical precision. This exact periodic example avoids leakage by placing every frequency on an integer bin; finite nonperiodic records need allowance for broadening and an [aperture](aperture.md).

For a continuous object field with [Fourier transform](fourier-transform-split.md) confined to $|f|\leq B$, the background $|O|^2$ occupies $|f|\leq2B$. A carrier $f_c>3B$ is a sufficient separation condition for the sideband centred at $-f_c$, and $f_c+B$ must remain below the [Nyquist spatial frequency](nyquist-spatial-frequency.md). Here $B=5$, $f_c=20$ and the [Nyquist spatial frequency](nyquist-spatial-frequency.md) is $512$. This sufficient bound describes a whole bandwidth, rather than exploiting the gaps in this particular two-component field.

The same example also makes optical playback explicit. Choose $t_0=0.3$ and $\beta=0.01$. Since $|O|\leq0.3$, the bounds $0.49\leq I\leq1.69$ imply $0.3049\leq t\leq0.3169$, and $|\beta I|/t_0\leq0.0564$. The affine response is stipulated; its weak-modulation interpretation is approximate. In $Rt$, the desired field $0.01O$ has frequencies $3,-5$; the conjugate term $0.01R^2O^*$ has frequencies $37,45$; the background has frequencies $20,12,28$. Thus the same carrier that separates the recorded cross terms separates the playback components. Reillumination restores a field through [diffraction](diffraction.md); computational filtering extracts the corresponding encoded field through [Fourier analysis](fourier-analysis-split.md).

## ↑ Ancestors (6)

1. [Holography](holography.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Aharonov-Bohm effect](aharonov-bohm-effect.md)
- [Holographic reference wave](holographic-reference-wave.md)
- [Off-axis holography](off-axis-holography.md)
- [Shielded toroidal-flux electron interference](shielded-toroidal-flux-electron-interference.md)
