<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

A [fixed space frame](../../../../../fixed-space-frame.md) is an inertial orthonormal frame whose axes remain fixed in space. A [principal body frame](../../../../../principal-body-frame.md) is attached to the rigid body and aligned with the principal axes of its inertia tensor, so that the tensor is diagonal with entries $I_1,I_2,I_3$.

If $e_i(t)$ are the body axes and $\omega$ is the [angular velocity](../../../../../angular-velocity.md), then the [derivative of a body-fixed basis vector](../../../../../derivative-of-a-body-fixed-basis-vector.md) is

$$
\dot e_i=\omega\times e_i.
$$

In the principal frame,

$$
L=\sum_{i=1}^3I_i\omega_i e_i.
$$

For torque-free motion, the [angular momentum](../../../../../angular-momentum.md) has zero space derivative. Therefore

$$
0=\frac{dL}{dt}
=\sum_iI_i\dot\omega_i e_i+\omega\times L.
$$

Taking body-frame components gives the [Euler equations for a torque-free rigid body](../../../../../euler-equations-for-a-torque-free-rigid-body.md):

$$
\begin{aligned}
I_1\dot\omega_1&=(I_2-I_3)\omega_2\omega_3,\\
I_2\dot\omega_2&=(I_3-I_1)\omega_3\omega_1,\\
I_3\dot\omega_3&=(I_1-I_2)\omega_1\omega_2.
\end{aligned}
$$

For an axisymmetric body, put $I_1=I_2=I$ and let $e_3$ be its symmetry axis. Decompose $\omega=\omega_1e_1+\omega_2e_2+\omega_3e_3$. Then

$$
\begin{aligned}
L
&=I\omega_1e_1+I\omega_2e_2+I_3\omega_3e_3\\
&=I\omega+(I_3-I)\omega_3e_3.
\end{aligned}
$$

**Thus $L$ is a linear combination of $\omega$ and $e_3$, proving that the angular momentum, angular velocity, and symmetry axis are always coplanar. This is the [coplanarity in a torque-free axisymmetric rigid body](../../../../../coplanarity-in-a-torque-free-axisymmetric-rigid-body.md).**

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
