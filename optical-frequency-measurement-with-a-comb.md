# Optical frequency measurement with a comb

↑ **Parent:** [Optical frequency comb](optical-frequency-comb.md)

Mix an unknown single-frequency [laser](laser-split.md) with a nearby comb tooth on a [photodiode](photodiode.md). Define the signed [beat](beat.md) $b=f_L-f_n$, so

$$
f_L=n f_r+f_0+b.
$$

The [beat](beat.md) arises from the cross term in [light intensity](light-intensity.md):

$$
\left|A e^{2\pi i f_Lt}+B e^{2\pi i f_nt}\right|^2
=|A|^2+|B|^2+2\operatorname{Re}\!\left(AB^*e^{2\pi i b t}\right).
$$

An electronic detector can follow this slow difference even though it cannot resolve either optical oscillation. The square-law expression also shows why a real-valued intensity trace by itself loses the sign of $b$. A small known upward shift of the chosen tooth decreases $|b|$ when the unknown lies above it and increases $|b|$ when it lies below, provided the tooth assignment remains unchanged.

For an original example, stipulate

$$
f_r=250\,\mathrm{MHz},\qquad f_0=20\,\mathrm{MHz},\qquad b=+30\,\mathrm{MHz},\qquad n=2{,}000{,}000.
$$

Then $f_n=500{,}000.020\,\mathrm{GHz}$ and $f_L=500{,}000.050\,\mathrm{GHz}$. Choosing the opposite sign would give $499{,}999.990\,\mathrm{GHz}$ instead. The stipulated optical [frequency](frequency.md) is countable because the large optical value is expressed using the [integer](integer-split.md) $n$ and three electronic [frequencies](frequency.md); the diagram's two controls establish the comb, and this additional [beat](beat.md) places the unknown against it.

Both comb readouts use one calibrated [microwave](microwave.md) reference. Feedback fixes $f_r$ and $f_0$, determining each tooth once $n$ is identified. A [frequency counter](frequency-counter.md) measures the slow [beat](beat.md), transferring the calibration to the optical [frequency](frequency.md).[Passion for Precision, p.158: microwave link](passion-for-precision-by-theodor-w-hansch.md)

**Table of contents**

- [Comb tooth index ambiguity](comb-tooth-index-ambiguity.md)

## ↑ Ancestors (6)

1. [Optical frequency comb](optical-frequency-comb.md)
2. [Laser](laser-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
