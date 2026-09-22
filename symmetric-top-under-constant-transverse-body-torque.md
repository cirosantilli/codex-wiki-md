# Symmetric top under constant transverse body torque

↑ **Parent:** [Symmetric top](symmetric-top.md)

Let a [symmetric top](symmetric-top.md) have [principal moments of inertia](principal-moment-of-inertia.md) $I_1=I_2=I_\perp$ and $I_3=I_\parallel$. Apply a [torque](torque.md) $(\tau_1,\tau_2,0)$ constant in a [principal body frame](principal-body-frame.md). Then the axial [angular velocity](angular-velocity.md) $c=\omega_3$ is a [conserved quantity](conserved-quantity.md). Define $z=\omega_1+i\omega_2$ and $\nu=(I_\parallel-I_\perp)c/I_\perp$. The first two of [Euler's equations](euler-s-equations-rigid-body-dynamics.md) combine into the equation in the title. This derivation uses constancy in the [principal body frame](principal-body-frame.md), which generally does not mean constant [torque](torque.md) in an [inertial frame](inertial-frame.md).

Multiplying by the [integrating factor](integrating-factor.md) $e^{-i\nu t}$ proves, for $\nu\ne0$,

$$
z(t)=z(0)e^{i\nu t}+\frac{\tau_1+i\tau_2}{i\nu I_\perp}(e^{i\nu t}-1).
$$

Equivalently $z$ rotates about the constant point $z_* =i(\tau_1+i\tau_2)/(\nu I_\perp)$ in the complex transverse plane. When $\nu=0$, the solution is instead $z(t)=z(0)+(\tau_1+i\tau_2)t/I_\perp$. The [angular velocity](angular-velocity.md) is $(\operatorname{Re}z,\operatorname{Im}z,c)$.

## ↑ Ancestors (6)

1. [Symmetric top](symmetric-top.md)
2. [Rigid body dynamics](rigid-body-dynamics-split.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-classical-mechanics-course-of-the-university-of-oxford/2023/2/b/iii/solution.md)
