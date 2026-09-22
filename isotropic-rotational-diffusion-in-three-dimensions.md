# Isotropic rotational diffusion in three dimensions

↑ **Parent:** [Rotational diffusion](rotational-diffusion.md)

For [isotropic](isotropy.md) turning in three dimensions, the tip of a marked [unit vector](unit-vector.md) $\mathbf u$ wanders over the unit [sphere](sphere.md). Its [probability density function](probability-density-function.md) $f$ obeys the orientational [Fokker-Planck equation](fokker-planck-equation.md)

$$
\frac{\partial f}{\partial t}=D_r\nabla_{\mathbf u}^2f,\qquad
C_1(t)=\langle\mathbf u(t)\cdot\mathbf u(0)\rangle=e^{-2D_rt},\qquad
\tau_1=\frac1{2D_r}.
$$

Here $\nabla_{\mathbf u}^2$ is the [Laplace-Beltrami operator](laplace-beltrami-operator.md) on the unit [sphere](sphere.md). The factor two follows from the [sphere surface derivative identities](sphere-surface-derivative-identities.md): $\nabla_{\mathbf u}^2u_i=-2u_i$, so each mean vector component decays at rate $2D_r$. This is a different orientation space from the circle of [planar rotational diffusion](planar-rotational-diffusion.md), whose corresponding rate is $D_r$. For the same illustrative $D_r=0.25\,\mathrm{s^{-1}}$ and $t=2\,\mathrm s$, this three-dimensional [autocorrelation](autocorrelation.md) is $e^{-1}\simeq0.368$.

One [unit vector](unit-vector.md) records a pointing direction, not every aspect of a [rigid body](rigid-body-dynamics-split.md)'s [rigid body orientation](rigid-body-orientation.md): rotation about that vector remains unspecified. Also, $C_1$ requires an identifiable arrow. An unmarked [ellipsoid](ellipsoid.md)'s long axis alone does not supply one, and projecting a three-dimensional trajectory onto a camera plane does not automatically produce the planar model.

## ↑ Ancestors (7)

1. [Rotational diffusion](rotational-diffusion.md)
2. [Diffusion](diffusion.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
