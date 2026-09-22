# Finite-volume angular source selection

↑ **Parent:** [Spontaneous symmetry breaking](spontaneous-symmetry-breaking.md)

Freeze the magnitude of an [order parameter](order-parameter.md) and retain just one common orientation $\theta$ for $N$ rigidly aligned cells. Give this collective coordinate [energy](energy-split.md) $E(\theta)=-Nh\cos\theta$ at positive [temperature](temperature-split.md) $T$. The [Boltzmann distribution](boltzmann-distribution.md) is the displayed normalized [probability density function](probability-density-function.md), where $k_B$ is the [Boltzmann constant](boltzmann-constant.md). Here $h$ is [energy](energy-split.md) per cell, a different normalization from the source density in [continuous vacuum selection by an external source](continuous-vacuum-selection-by-an-external-source.md). This is a deliberately restricted model of selection among already ordered orientations: it does not derive alignment or an ordering [critical temperature](critical-temperature.md) from a spatial interaction.

Its mean orientation is an elementary ratio of integrals:

$$
m_N(h)=\langle\cos\theta\rangle=\frac{\int_{-\pi}^{\pi}\cos\theta\,e^{x\cos\theta}\,d\theta}{\int_{-\pi}^{\pi}e^{x\cos\theta}\,d\theta}.
$$

At $h=0$ every angle has equal [probability](probability.md), and the numerator vanishes exactly. For small $x$, expansion of the exponential gives $m_N(h)=x/2+O(x^3)$ because the angular mean of $\cos^2\theta$ is $1/2$. For $x=1$ and $5$ the means are approximately $0.446390$ and $0.893383$. At fixed $h>0$, increasing $N$ concentrates the [probability density function](probability-density-function.md) near $\theta=0$; expanding $\cos\theta=1-\theta^2/2+O(\theta^4)$ gives angular [variance](variance-split.md) approximately $1/x$. Consequently

$$
\lim_{h\downarrow0}\lim_{N\to\infty}m_N(h)=1,\qquad
\lim_{N\to\infty}\lim_{h\to0}m_N(h)=0.
$$

The uniform angular average remains a symmetric mixture if one sets $h=0$ first. The other order selects a definite direction. This is the continuous-orientation version of the [symmetry-breaking order of limits](symmetry-breaking-order-of-limits.md); it illustrates selection without replacing the separate problem of stability against spatial fluctuations.

<a id="image-one-collective-angle-illustrates-noncommuting-source-and-size-limits"></a>
![](continuous-symmetry-source-selection.png)

**[Figure 2](#image-one-collective-angle-illustrates-noncommuting-source-and-size-limits). One collective angle illustrates noncommuting source and size limits**. Original normalized [Boltzmann distribution](boltzmann-distribution.md) integrals for the rigid-orientation model. Every finite-$N$ response curve passes through zero at zero source. At fixed positive source, increasing $N$ narrows the angular [probability density function](probability-density-function.md). These curves are model calculations, not measured data or an independent derivation of a thermodynamic ordered phase.

## ↑ Ancestors (5)

1. [Spontaneous symmetry breaking](spontaneous-symmetry-breaking.md)
2. [Quantum field theory](quantum-field-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Spontaneous symmetry breaking](spontaneous-symmetry-breaking.md)
