# Dirty image

↑ **Parent:** [Dirty beam](dirty-beam.md)

The dirty image is the direct weighted inverse [Fourier transform](fourier-transform-split.md) of the measured [complex visibilities](complex-visibility.md):

$$
I_D(\theta)=\frac{1}{W}\sum_k w_k V(u_k)e^{2\pi i u_k\theta}
=\sum_j I_jB(\theta-\theta_j).
$$

The final equality follows by substituting the point-source [complex visibility](complex-visibility.md) and exchanging the finite sums. For continuous brightness it is a [convolution](convolution.md) with the [dirty beam](dirty-beam.md), with the [primary beam](primary-beam.md) included in the brightness when necessary. Negative values and subsidiary peaks can arise from that response even when every true source has positive strength.

**Table of contents**

- [Two-point-source aperture synthesis](two-point-source-aperture-synthesis.md)

## ↑ Ancestors (8)

1. [Dirty beam](dirty-beam.md)
2. [Aperture synthesis](aperture-synthesis.md)
3. [Radio astronomy](radio-astronomy.md)
4. [Observational astronomy](observational-astronomy.md)
5. [Astrophysics](astrophysics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Two-point-source aperture synthesis](two-point-source-aperture-synthesis.md)
