# Fourier solution of a loaded elastic half-space

↑ **Parent:** [Airy stress function](airy-stress-function.md)

For plane strain in $y>0$ under surface normal traction $-P(x)$ and zero surface shear, use the forward [Fourier transform](fourier-transform-split.md) phase $e^{ikx}$. At $k\ne0$, biharmonicity gives $(\partial_y^2-k^2)^2\widehat A=0$, whose decaying part is $(C+Dy)e^{-|k|y}$. Boundary traction fixes $C=\widehat P/k^2$, $D=|k|C$, proving the displayed formula. Constitutive inversion and a decaying displacement mode give $2\mu\widehat v=[y+2(1-\nu)/|k|]\widehat P e^{-|k|y}$. Multiplication by $-ik$ produces an unambiguous displacement-gradient convolution kernel.

The zero mode is separate: a nonzero resultant load $\widehat P(0)$ conflicts with an ordinary fully decaying displacement normalization in two dimensions and leads to a logarithmic reference issue. Balanced loading or a distributional/reference-displacement treatment is required before extending the transformed formulas globally. Dividing by $k^2$ and assigning a finite value at $k=0$ is invalid.

## ↑ Ancestors (8)

1. [Airy stress function](airy-stress-function.md)
2. [Plane strain](plane-strain.md)
3. [Finite strain theory](finite-strain-theory.md)
4. [Deformation (mechanics)](deformation-mechanics.md)
5. [Continuum mechanics](continuum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-elasticity-and-plasticity-course-of-the-university-of-oxford/2009/2/b/ii/solution.md)
