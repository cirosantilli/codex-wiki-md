<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

The components in [Euler equations for a torque-free rigid body](../../../../../euler-equations-for-a-torque-free-rigid-body.md) are evaluated in the body-fixed principal-axis frame, with $L_i=I_i\omega_i$. In an inertial space frame the [angular momentum](../../../../../angular-momentum.md) vector is constant; its components in the rotating body frame need not be.

Assume $\Omega\ne0$ and distinct positive [principal moments of inertia](../../../../../principal-moment-of-inertia.md). Write $\omega=(\Omega+\delta_1,\delta_2,\delta_3)$. To first order,

$$
\dot\delta_1=0,\qquad
\dot\delta_2=\frac{I_3-I_1}{I_2}\Omega\delta_3,
\qquad\dot\delta_3=\frac{I_1-I_2}{I_3}\Omega\delta_2,
$$

so

$$
\ddot\delta_2=\Omega^2\frac{(I_3-I_1)(I_1-I_2)}{I_2I_3}\delta_2.
$$

The coefficient is positive when $I_1$ lies between the other moments, giving an exponentially growing mode and instability. When $I_1$ is an extreme moment, it is negative and the transverse perturbations oscillate.

To establish actual nonlinear [Lyapunov stability](../../../../../lyapunov-stability.md) in the latter case, use the conserved [kinetic energy](../../../../../kinetic-energy.md) $E=\frac12\sum I_j\omega_j^2$ and squared [angular momentum](../../../../../angular-momentum.md) $L^2=\sum I_j^2\omega_j^2$. Their combination is

$$
L^2-2I_1E=I_2(I_2-I_1)\omega_2^2+I_3(I_3-I_1)\omega_3^2.
$$

For an extreme $I_1$ its two coefficients have the same sign. Conservation controls both transverse components by their initially small values, while conservation of $E$ controls $\omega_1^2$ near $\Omega^2$. [Continuity](../../../../../continuous-function.md) preserves its initial sign for sufficiently small perturbations. Thus **nonzero steady rotation is stable exactly about the largest or smallest principal moment**, the [intermediate axis theorem](../../../../../intermediate-axis-theorem.md). It is not asymptotically stable, since [energy](../../../../../energy.md) is conserved. If $\Omega=0$, [energy](../../../../../energy.md) makes the zero angular-velocity state stable for every ordering; the nonzero-rotation assumption is essential to the stated equivalence.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
