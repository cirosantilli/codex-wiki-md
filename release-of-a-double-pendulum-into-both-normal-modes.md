# Release of a double pendulum into both normal modes

↑ **Parent:** [Normal modes of a double pendulum](normal-modes-of-a-double-pendulum.md)

Release the upper rod at $\theta_1(0)=\alpha=0.06$ radians while keeping the lower rod vertical, $\theta_2(0)=0$, with both [angular velocities](angular-velocity.md) zero. The [initial condition](initial-condition.md) is the sum $\boldsymbol\theta(0)=(\alpha/2)\mathbf a_-+(\alpha/2)\mathbf a_+$. The solution from [linearization](linearization.md) is therefore

$$
\begin{aligned}
\theta_1(t)&=\frac\alpha2\left[\cos(\omega_-t)+\cos(\omega_+t)\right],\\
\theta_2(t)&=\frac\alpha{\sqrt2}\left[\cos(\omega_-t)-\cos(\omega_+t)\right].
\end{aligned}
$$

At release the lower [angle](angle.md) vanishes by cancellation between the two [normal modes](normal-mode.md). Their different [angular frequencies](angular-frequency.md) then destroy that cancellation. Differentiating twice gives $\ddot\theta_1(0)=-2g\alpha/\ell$ and $\ddot\theta_2(0)=2g\alpha/\ell$, agreeing with the small-[angle](angle.md) limit of the exact [double pendulum equations of motion](double-pendulum-equations-of-motion.md).

The quadratic [mechanical energy](mechanical-energy.md) at release is $E_2=mg\ell\alpha^2$. Each [normal mode](normal-mode.md) contributes half, because $(4+2\sqrt2)(2-\sqrt2)=(4-2\sqrt2)(2+\sqrt2)=4$. Equal coordinate [amplitudes](wave-amplitude.md) need not mean equal [energies](energy-split.md) in general; here the modal inertias and squared [angular frequencies](angular-frequency.md) happen to compensate. Releasing instead along $\boldsymbol\theta(0)=\alpha\mathbf a_-$ or $\alpha\mathbf a_+$, with zero [angular velocities](angular-velocity.md), excites just one [normal mode](normal-mode.md).

## ↑ Ancestors (8)

1. [Normal modes of a double pendulum](normal-modes-of-a-double-pendulum.md)
2. [Generalized eigenvalue problem for small oscillations](generalized-eigenvalue-problem-for-small-oscillations.md)
3. [Small oscillation](small-oscillation.md)
4. [Lagrangian mechanics](lagrangian-mechanics-split.md)
5. [Classical mechanics](classical-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
