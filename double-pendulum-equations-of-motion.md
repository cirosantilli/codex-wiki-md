# Double pendulum equations of motion

↑ **Parent:** [Double pendulum](double-pendulum.md)

Write $\Delta=\theta_1-\theta_2$. Applying the [Euler-Lagrange equations](euler-lagrange-equation.md) to the [double pendulum Lagrangian](double-pendulum-lagrangian.md), then dividing by $m\ell^2$, gives

$$
\begin{aligned}
2\ddot\theta_1+\cos\Delta\,\ddot\theta_2+\sin\Delta\,\dot\theta_2^2+\frac{2g}{\ell}\sin\theta_1&=0,\\
\cos\Delta\,\ddot\theta_1+\ddot\theta_2-\sin\Delta\,\dot\theta_1^2+\frac{g}{\ell}\sin\theta_2&=0.
\end{aligned}
$$

For example, the upper [generalized momentum](generalized-momentum.md) is $\partial L/\partial\dot\theta_1=m\ell^2(2\dot\theta_1+\cos\Delta\,\dot\theta_2)$. Its [time](time-in-physics.md) derivative contains $-m\ell^2\sin\Delta(\dot\theta_1-\dot\theta_2)\dot\theta_2$. Subtracting $\partial L/\partial\theta_1=-m\ell^2\sin\Delta\,\dot\theta_1\dot\theta_2-2mg\ell\sin\theta_1$ cancels the mixed product and leaves the positive $\sin\Delta\,\dot\theta_2^2$ term in the first equation. This cancellation is a useful check on the sign convention.

The [matrix](matrix.md) multiplying the two angular [accelerations](acceleration.md) is

$$
\begin{pmatrix}2&\cos\Delta\\\cos\Delta&1\end{pmatrix},\qquad
\det=2-\cos^2\Delta\geq1.
$$

It is invertible for every configuration, so specified [angles](angle.md) and [angular velocities](angular-velocity.md) determine both angular [accelerations](acceleration.md). For the same reason $T>0$ whenever the [angular velocities](angular-velocity.md) are not both zero. The [mass](mass.md) cancels from the motion equations, while the timescale is set by $\sqrt{\ell/g}$.

As an exact constructed release, put $\theta_1(0)=\alpha$, $\theta_2(0)=0$, and both [angular velocities](angular-velocity.md) zero. Solving the two equations at release yields

$$
\ddot\theta_1(0)=-\frac{2g}{\ell}\frac{\sin\alpha}{2-\cos^2\alpha},\qquad
\ddot\theta_2(0)=\frac{2g}{\ell}\frac{\sin\alpha\cos\alpha}{2-\cos^2\alpha}.
$$

For $0<\alpha<\pi/2$, the upper rod initially moves back toward vertical, while the lower rod initially moves away from it. The lower pivot's [acceleration](acceleration.md) makes this possible even though the lower rod starts vertical. The [small-angle approximation](small-angle-approximation.md) gives $\ddot\theta_1(0)\simeq-2g\alpha/\ell$ and $\ddot\theta_2(0)\simeq2g\alpha/\ell$.

The conserved [mechanical energy](mechanical-energy.md) is $E=T+V$, because the [Lagrangian](lagrangian.md) has no explicit [time](time-in-physics.md) dependence. Directly, $dE/dt$ is $m\ell^2$ times the first equation multiplied by $\dot\theta_1$ plus the second multiplied by $\dot\theta_2$, so the equations imply $dE/dt=0$. This also supplies a check when computing a [trajectory](trajectory.md).

## ↑ Ancestors (6)

1. [Double pendulum](double-pendulum.md)
2. [Lagrangian mechanics](lagrangian-mechanics-split.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Normal modes of a double pendulum](normal-modes-of-a-double-pendulum.md)
- [Release of a double pendulum into both normal modes](release-of-a-double-pendulum-into-both-normal-modes.md)
