# Dirty beam

↑ **Parent:** [Aperture synthesis](aperture-synthesis.md)

The dirty beam is the [point spread function](point-spread-function-split.md) obtained by directly inverting the weighted sampled [complex visibilities](complex-visibility.md). For sampling positions $u_k$ and nonnegative weights $w_k$ with $W=\sum_k w_k>0$, choose

$$
B(\theta)=\frac{1}{W}\sum_k w_ke^{2\pi i u_k\theta},\qquad B(0)=1.
$$

Include each $u_k$ with $-u_k$ and the same weight so that $B$ is real. Its unit peak convention means that an isolated unit point source contributes a shifted unit-height response. It is not a unit-integral convention. Sparse sampling can leave substantial subsidiary peaks, even when the longest [interferometric baseline](interferometric-baseline.md) is large.

**Table of contents**

- [Dirty image](dirty-image.md)
  - [Two-point-source aperture synthesis](two-point-source-aperture-synthesis.md)

## ↑ Ancestors (7)

1. [Aperture synthesis](aperture-synthesis.md)
2. [Radio astronomy](radio-astronomy.md)
3. [Observational astronomy](observational-astronomy.md)
4. [Astrophysics](astrophysics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Dirty image](dirty-image.md)
- [Primary beam](primary-beam.md)
- [Two-point-source aperture synthesis](two-point-source-aperture-synthesis.md)
