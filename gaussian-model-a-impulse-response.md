# Gaussian Model A impulse response

↑ **Parent:** [Nonconserved order-parameter dynamics](nonconserved-order-parameter-dynamics.md)

For quadratic [free energy](thermodynamic-free-energy.md) with positive $a,\kappa$ and [kinetic coefficient](kinetic-coefficient.md) $\Gamma$, a deterministic initial [Dirac delta distribution](dirac-delta-function.md) evolves under [nonconserved order-parameter dynamics](nonconserved-order-parameter-dynamics.md) to the mean

$$
\langle\phi(\mathbf r,t)\rangle=\frac{Ae^{-\Gamma at}}{(4\pi\Gamma\kappa t)^{d/2}}e^{-|\mathbf r-\mathbf r'|^2/(4\Gamma\kappa t)}.
$$

Taking the expectation removes the centered [Gaussian white noise](gaussian-white-noise.md); the resulting diffusion-reaction equation is solved by the [heat kernel](heat-kernel.md). The integrated mean is $Ae^{-\Gamma at}$, so spreading does not conserve the initial excess. The connected [Fourier mode](fourier-mode.md) covariance grows from zero to $k_BT/(a+\kappa q^2)$ as $1-e^{-2\Gamma(a+\kappa q^2)t}$ by the [Itô isometry](ito-isometry.md). A realization retains equilibrium fluctuations after its mean has decayed. Pointwise continuum white-noise quantities require a coarse-graining cutoff.

## ↑ Ancestors (7)

1. [Nonconserved order-parameter dynamics](nonconserved-order-parameter-dynamics.md)
2. [Order parameter](order-parameter.md)
3. [Critical phenomenon](critical-phenomenon-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344/1/e/solution.md)
