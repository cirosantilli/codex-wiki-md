# Nuclear charge form factor

↑ **Parent:** [Nuclear charge distribution](nuclear-charge-distribution.md)

In the static [charge density](charge-density.md) model, define the normalized [Fourier transform](fourier-transform-split.md)

$$
F(\mathbf q)=\frac1{Ze}\int\rho_{\mathrm{ch}}(\mathbf r)e^{i\mathbf q\cdot\mathbf r}\,d^3r,
\qquad F(\mathbf 0)=1.
$$

Here $\mathbf q=(\mathbf p-\mathbf p')/\hbar$ is the spatial [momentum transfer](momentum-transfer.md) divided by the reduced [Planck constant](planck-constant.md): $q=|\mathbf q|$ has units of inverse length. Physical [momentum transfer](momentum-transfer.md) is $\hbar\mathbf q$. We keep $\hbar$ and the [speed of light](speed-of-light.md) $c$ explicit; compute $q=|\mathbf p-\mathbf p'|c/(\hbar c)$, expressing the numerator in $\mathrm{MeV}$ and $\hbar c$ in $\mathrm{MeV}\,\mathrm{fm}$, to obtain $q$ in inverse [femtometres](femtometre.md). The spatial $q$ is distinct from the invariant [four-momentum](four-momentum.md) transfer used in [relativistic scattering cross-sections](relativistic-scattering-cross-section.md).

For [spherical symmetry](spherical-symmetry.md), take the polar axis along $\mathbf q$ and use [spherical coordinates](spherical-coordinate-system.md). With $\mu$ the cosine of the polar angle,

$$
\int_{-1}^{1}e^{iqr\mu}\,d\mu=2\frac{\sin(qr)}{qr},
\qquad
F(q)=\frac{4\pi}{Ze}\int_0^\infty r^2\rho_{\mathrm{ch}}(r)\frac{\sin(qr)}{qr}\,dr.
$$

Every radial shell contributes an amplitude. At $q=0$ all shells add with the same sign; at larger $q$ their contributions can cancel. This cancellation is the origin of a [diffraction](diffraction.md) minimum in the [nuclear charge form factor](nuclear-charge-form-factor.md), rather than an absence of [electric charge](electric-charge-split.md) in the [nucleus](atomic-nucleus-split.md).

The static [Fourier transform](fourier-transform-split.md) interpretation is appropriate for the nuclear model and kinematic regime specified here. A fully relativistic composite system requires frame and current conventions; its electric form factor is not universally the transform of a frame-independent three-dimensional [charge density](charge-density.md).

**Table of contents**

- [Uniform-sphere nuclear charge form factor](uniform-sphere-nuclear-charge-form-factor.md)
- [Nuclear elastic electron scattering cross-section](nuclear-elastic-electron-scattering-cross-section.md)

## ↑ Ancestors (5)

1. [Nuclear charge distribution](nuclear-charge-distribution.md)
2. [Atomic nucleus](atomic-nucleus-split.md)
3. [Nuclear physics](nuclear-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Hofstadter nuclear electron scattering experiment](hofstadter-nuclear-electron-scattering-experiment.md)
- [Nuclear charge form factor](nuclear-charge-form-factor.md)
- [Nuclear charge radius](nuclear-charge-radius.md)
- [Solution](past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2012/paper-1/2/c/solution.md)
- [Solution](past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2017/2/a/solution.md)
- [Uniform-sphere nuclear charge form factor](uniform-sphere-nuclear-charge-form-factor.md)
