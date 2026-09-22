# Delay quantization and bandwidth decorrelation

↑ **Parent:** [Radio interferometry](radio-interferometry.md)

A residual delay $\delta\tau$ in a rectangular band of width $\Delta\nu$ attenuates the correlated amplitude by $\operatorname{sinc}(\pi\Delta\nu\delta\tau)$. Coarse delay quantization must keep this factor near one; the relevant path scale is $c/\Delta\nu$. Separately, an untracked carrier phase has error $2\pi\delta\ell/\lambda$. Fine phase rotation can remove that central-frequency phase while leaving the band-dependent decorrelation, so delay-step specifications must state both [bandwidth](bandwidth-signal-processing.md) and compensation architecture.

## ↑ Ancestors (8)

1. [Radio interferometry](radio-interferometry.md)
2. [Aperture synthesis](aperture-synthesis.md)
3. [Radio astronomy](radio-astronomy.md)
4. [Observational astronomy](observational-astronomy.md)
5. [Astrophysics](astrophysics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
