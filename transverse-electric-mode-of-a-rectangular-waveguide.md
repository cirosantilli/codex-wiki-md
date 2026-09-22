# Transverse electric mode of a rectangular waveguide

↑ **Parent:** [Rectangular electromagnetic waveguide](rectangular-electromagnetic-waveguide.md)

A [transverse electric mode of a rectangular waveguide](transverse-electric-mode-of-a-rectangular-waveguide.md) has $E_z=0$ while its axial [magnetic field](magnetic-field-split.md) is generally nonzero. For time dependence $e^{-i\omega t}$ and axial dependence $e^{i\beta z}$, set $\Delta=(\omega/c)^2-\beta^2$. The [Maxwell equations](maxwell-equations-split.md) reconstruct the transverse components from $B_z$:

$$
B_x=\frac{i\beta}{\Delta}\partial_xB_z,\quad
B_y=\frac{i\beta}{\Delta}\partial_yB_z,\quad
E_x=\frac{i\omega}{\Delta}\partial_yB_z,\quad
E_y=-\frac{i\omega}{\Delta}\partial_xB_z.
$$

The axial [complex amplitude](complex-amplitude.md) satisfies a transverse [Helmholtz equation](helmholtz-equation.md), $(\partial_x^2+\partial_y^2+\Delta)B_z=0$. Zero tangential [electric field](electric-field-split.md) at each [perfect conductor](perfect-conductor.md) wall becomes a [Neumann boundary condition](neumann-boundary-condition.md) on $B_z$. [Separation of variables](separation-of-variables.md) gives

$$
B_z=B_*\cos(m\pi x/a)\cos(n\pi y/b)e^{i\beta z},\qquad \Delta=\kappa_{mn}^2.
$$

The index $m$ counts half-periods across $a$, and $n$ across $b$. Either index can vanish, allowing $\mathrm{TE}_{10}$; both cannot vanish. Indeed a spatially constant axial oscillating [magnetic field](magnetic-field-split.md) would give nonzero changing [magnetic flux](magnetic-flux.md) through the cross-section, whereas the [line integral](line-integral.md) of tangential [electric field](electric-field-split.md) around its metal boundary is zero. The integral form of [Faraday's law](faraday-s-law-of-induction.md) excludes this $\mathrm{TE}_{00}$ candidate. Dividing the reconstruction formulas by $\Delta=0$ would be invalid and cannot produce the separate [transverse electromagnetic mode](transverse-electromagnetic-mode.md).

For $m=1,n=0$, choose $B_*=-i(\pi/a)E_0/\omega$. The formulas recover exactly the $E_y$, $B_x$ and $B_z$ in [rectangular electromagnetic waveguide](rectangular-electromagnetic-waveguide.md). In particular, the transverse [magnetic field](magnetic-field-split.md) accompanies $B_z$ and ensures zero [divergence](divergence.md); an oscillating longitudinal [magnetic field](magnetic-field-split.md) on its own is not the guided solution.

**Table of contents**

- [Evanescent transverse electric mode in a rectangular waveguide](evanescent-transverse-electric-mode-in-a-rectangular-waveguide.md)

## ↑ Ancestors (6)

1. [Rectangular electromagnetic waveguide](rectangular-electromagnetic-waveguide.md)
2. [Electromagnetic wave](electromagnetic-wave-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/17a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1/section-d/d12/c/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1/section-a/a3/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1/section-b/b9/solution.md)
- [Rectangular electromagnetic waveguide](rectangular-electromagnetic-waveguide.md)
- [Transverse electric mode of a rectangular waveguide](transverse-electric-mode-of-a-rectangular-waveguide.md)
- [Waveguide cutoff frequency](waveguide-cutoff-frequency.md)
