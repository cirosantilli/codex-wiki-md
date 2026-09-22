# Poisson variance after sky subtraction

↑ **Parent:** [Signal-to-noise ratio in photon counting](signal-to-noise-ratio-in-photon-counting.md)

Subtracting an exactly known mean sky level leaves source-plus-sky [variance](variance-split.md) of a [Poisson distribution](poisson-distribution.md) $S+B$. If the sky per source [pixel](pixel.md) is estimated from $n_b$ equal-area, equally exposed independent sky [pixels](pixel.md), its additional [variance](variance-split.md) is $B/n_b$, so $R=S/\sqrt{S+B+B/n_b}$ before read and dark terms. The [variance](variance-split.md) of removed background [photons](photon.md) does not disappear with their mean.

## ↑ Ancestors (7)

1. [Signal-to-noise ratio in photon counting](signal-to-noise-ratio-in-photon-counting.md)
2. [Photodetector](photodetector.md)
3. [Optical instrument](optical-instrument-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
