# Gain estimation from flat-field ratios

↑ **Parent:** [Detector conversion gain](detector-conversion-gain.md)

Let independent exposure sums $A,B$ have mean $N$ [ADU](analogue-to-digital-unit.md) at each [detector pixel](optical-detector-pixel.md), with pure [Poisson distribution](poisson-distribution.md) noise and fixed gain $g$. The [delta method](delta-method.md) gives $A/B\simeq1+(A-N)/N-(B-N)/N$, so $\operatorname{Var}(A/B)\simeq2/(gN)$ and $g\simeq2/(NE^2)$. For nonuniform [detector pixel](optical-detector-pixel.md) means $N_i$, an unweighted spatial ratio [variance](variance-split.md) is instead $(2/g)\langle1/N_i\rangle$. This high-count approximation requires linear unsaturated data, bias subtraction and negligible [read noise](read-noise.md).

**Table of contents**

- [Bias of pooled flat-field ratio gain](bias-of-pooled-flat-field-ratio-gain.md)

## ↑ Ancestors (7)

1. [Detector conversion gain](detector-conversion-gain.md)
2. [Photodetector](photodetector.md)
3. [Optical instrument](optical-instrument.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/3/c/i/solution.md)
