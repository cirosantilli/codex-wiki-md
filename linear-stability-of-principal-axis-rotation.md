# Linear stability of principal-axis rotation

↑ **Parent:** [Intermediate axis theorem](intermediate-axis-theorem.md)

For $0<I_1<I_2<I_3$, the transverse [linear stability](linear-stability.md) rates about steady rotation with signed component $\Omega\ne0$ are

$$
\nu_1=|\Omega|\sqrt{\frac{(I_2-I_1)(I_3-I_1)}{I_2I_3}},\qquad
\nu_3=|\Omega|\sqrt{\frac{(I_3-I_2)(I_3-I_1)}{I_1I_2}},\qquad
\lambda_2=|\Omega|\sqrt{\frac{(I_2-I_1)(I_3-I_2)}{I_1I_3}}.
$$

Axes one and three have transverse [eigenvalues](eigenvalue.md) $\pm i\nu_1$ and $\pm i\nu_3$, producing bounded [oscillations](oscillation.md). Axis two has transverse [eigenvalues](eigenvalue.md) $\pm\lambda_2$, giving growing and decaying [exponential functions](exponential-function.md). A neutral longitudinal [perturbation](perturbation.md) corresponds to a small change of $\Omega$. Generic intermediate-axis disturbances contain a growing component; a precisely chosen decaying direction is exceptional. For the [normalized intermediate-axis model](normalized-intermediate-axis-model.md) with $|\Omega|=1$, the values are $\nu_1=1/\sqrt3$, $\nu_3=1$ and $\lambda_2=1/\sqrt3$.

Proof outline: the [linearization](linearization.md) of the [Euler equations for a torque-free rigid body](euler-equations-for-a-torque-free-rigid-body.md) about the third [principal axis](principal-axis.md) gives transverse [perturbations](perturbation.md) obeying

$$
\dot\omega_1=\frac{I_2-I_3}{I_1}\Omega\omega_2,\qquad
\dot\omega_2=\frac{I_3-I_1}{I_2}\Omega\omega_1,
$$

and hence

$$
\ddot\omega_1=-\Omega^2\frac{(I_3-I_2)(I_3-I_1)}{I_1I_2}\omega_1.
$$

Cyclic permutation gives the other rates. For nonlinear [Lyapunov stability](lyapunov-stability.md) of the extreme rotations, use the [torque-free rigid-body invariants](torque-free-rigid-body-invariants.md): the conserved [quadratic forms](quadratic-form-split.md) $L^2-2I_1E$ and $2I_3E-L^2$ have strictly positive transverse coefficients about axes one and three respectively. They bound transverse [angular velocity](angular-velocity.md), while $E$ bounds its longitudinal change near nonzero rotation. Imaginary transverse [eigenvalues](eigenvalue.md) alone would not establish this nonlinear conclusion.[Classical Dynamics by David Tong, §3.4.3, equations (3.41)–(3.45), and §3.4.4, invariants (3.46)–(3.47); the invariant-bound argument here is an original short derivation](classical-dynamics-by-david-tong/3-the-motion-of-rigid-bodies.md)

The practical lesson is to choose a stable [principal axis](principal-axis.md) when using rotation to maintain an instrument's pointing direction. Both extreme [principal moments of inertia](principal-moment-of-inertia.md) are stable in the ideal torque-free model; if internal [damping](damping.md) lowers [rotational kinetic energy](rotational-kinetic-energy.md) while approximately preserving [angular momentum](angular-momentum.md), the minimum energy $E=L^2/(2I_3)$ instead favors the largest [principal moment of inertia](principal-moment-of-inertia.md). A control system must account for [torque](torque.md), changing [mass](mass.md) distributions and flexibility before applying this ideal result.

## ↑ Ancestors (8)

1. [Intermediate axis theorem](intermediate-axis-theorem.md)
2. [Euler equations for a torque-free rigid body](euler-equations-for-a-torque-free-rigid-body.md)
3. [Euler's equations (rigid body dynamics)](euler-s-equations-rigid-body-dynamics.md)
4. [Rigid body dynamics](rigid-body-dynamics-split.md)
5. [Classical mechanics](classical-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/8e/c/solution.md)
