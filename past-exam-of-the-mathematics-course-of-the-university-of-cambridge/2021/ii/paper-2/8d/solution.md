<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

Let $R$ be the [center of mass](../../../../../center-of-mass.md) and $g$ the uniform gravitational acceleration. The gravitational [torque](../../../../../torque.md) about $R$ is

$$
\sum_i(r_i-R)\times m_i g
=\left(\sum_i m_i(r_i-R)\right)\times g=0.
$$

Choose body-fixed [principal axes of inertia](../../../../../principal-body-frame.md). The inertial derivative of the [angular momentum](../../../../../angular-momentum.md) is

$$
N=\left(\frac{dL}{dt}\right)_{\rm body}+\omega\times L.
$$

For torque-free motion $N=0$ and $L_i=I_i\omega_i$, giving the [Euler equations for a torque-free rigid body](../../../../../euler-equations-for-a-torque-free-rigid-body.md)

$$
\begin{aligned}
I_1\dot\omega_1+(I_3-I_2)\omega_2\omega_3&=0,\\
I_2\dot\omega_2+(I_1-I_3)\omega_3\omega_1&=0,\\
I_3\dot\omega_3+(I_2-I_1)\omega_1\omega_2&=0.
\end{aligned}
$$

For a [symmetric top](../../../../../symmetric-top.md), let $I_1=I_2=I$ and let $I_3$ be the axial moment. Then $\omega_3$ is constant and

$$
\dot\omega_1=-\Omega\omega_2,
\qquad
\dot\omega_2=\Omega\omega_1,
\qquad
\Omega=\frac{I_3-I}{I}\omega_3.
$$

Thus $\omega_1^2+\omega_2^2$ is constant and the transverse angular-velocity vector rotates uniformly about the body symmetry axis. Its rate is $|\Omega|$; it precesses in the positive axial sense when $(I_3-I)\omega_3>0$ and in the opposite sense when this product is negative.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
