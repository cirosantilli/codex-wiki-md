# Bias of pooled flat-field ratio gain

↑ **Parent:** [Gain estimation from flat-field ratios](gain-estimation-from-flat-field-ratios.md)

For stable positive [detector pixel](optical-detector-pixel.md) means $N_i$ and uniform [detector conversion gain](detector-conversion-gain.md) $g$, high-count independent [Poisson distribution](poisson-distribution.md) noise gives $\operatorname{Var}(A_i/B_i)\simeq2/(gN_i)$. Thus substituting a global mean in the equal-signal formula yields $g_{\rm naive}=g/[\langle N_i\rangle\langle1/N_i\rangle]\le g$, by the [Jensen inequality](jensen-s-inequality.md). Equality holds for uniform means. The [flat-field correction](flat-field-correction.md) pattern cancels from the ratio mean but not from the signal-dependent noise. Local signal bins, or a [variance](variance-split.md) fit after normalization of differences by the square root of their local mean, avoid this leading bias.

## ↑ Ancestors (8)

1. [Gain estimation from flat-field ratios](gain-estimation-from-flat-field-ratios.md)
2. [Detector conversion gain](detector-conversion-gain.md)
3. [Photodetector](photodetector.md)
4. [Optical instrument](optical-instrument.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
