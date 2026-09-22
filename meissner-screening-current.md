# Meissner screening current

↑ **Parent:** [Planar London screening](planar-london-screening.md)

In [SI](international-system-of-units.md) units, the [magnetostatic Ampère law](magnetostatic-ampere-law.md) gives the [current density](current-density.md) supporting [Planar London screening](planar-london-screening.md):

$$
\mathbf J=\frac{1}{\mu_0}\nabla\times\mathbf B
=-\frac{B_0}{\mu_0\lambda_L}e^{-z/\lambda_L}\widehat{\mathbf y}.
$$

Here $\mu_0$ is the [vacuum permeability](vacuum-permeability.md). The sign follows from $(\nabla\times\mathbf B)_y=\partial_zB_x$ in the chosen coordinates. Thus $B_0>0$ requires [electric current](electric-current.md) along $-\widehat{\mathbf y}$. Its own [magnetic field](magnetic-field-split.md) opposes the imposed [magnetic field](magnetic-field-split.md) inside the material. The [electric current](electric-current.md) is distributed over a finite layer; its depth [integral](integral-split.md) is the effective [surface current density](surface-current-density.md)

$$
\mathbf K=\int_0^\infty\mathbf J(z)\,dz
=-\frac{B_0}{\mu_0}\widehat{\mathbf y}.
$$

The units are $\mathrm{A\,m^{-2}}$ for $\mathbf J$ and $\mathrm{A\,m^{-1}}$ for $\mathbf K$. Shrinking $\lambda_L$ at fixed $B_0$ increases the surface [current density](current-density.md), while this integrated [surface current density](surface-current-density.md) stays fixed. The [current sheet](current-sheet.md) approximation is the large-length-scale limit of this layer, not a claim that an actual sample carries an infinitely thin [electric current](electric-current.md). It reproduces the [magnetic-field jump across a surface current](magnetic-field-jump-across-a-surface-current.md) between the exterior $B_0\widehat{\mathbf x}$ and a field-free interior, with outward [unit normal](unit-normal.md) $-\widehat{\mathbf z}$.

## ↑ Ancestors (9)

1. [Planar London screening](planar-london-screening.md)
2. [Meissner state](meissner-state.md)
3. [Meissner effect](meissner-effect.md)
4. [London equations](london-equations.md)
5. [Magnetic field](magnetic-field-split.md)
6. [Electromagnetism](electromagnetism-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Planar London screening](planar-london-screening.md)
