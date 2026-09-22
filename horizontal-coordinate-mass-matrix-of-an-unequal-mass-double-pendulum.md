# Horizontal-coordinate mass matrix of an unequal-mass double pendulum

↑ **Parent:** [Normal modes of a double pendulum](normal-modes-of-a-double-pendulum.md)

For equal rod lengths $l$, upper [mass](mass.md) $m$ and lower [mass](mass.md) $\alpha m>0$, use horizontal [displacements](displacement.md) $x_1=l\theta_1$, $x_2=l(\theta_1+\theta_2)$ at first order. The quadratic [kinetic energy](kinetic-energy.md) is $m\dot x_1^2/2+\alpha m\dot x_2^2/2$, while the [stiffness matrix](stiffness-matrix.md) is

$$
K=\frac{mg}{l}\begin{pmatrix}1+2\alpha&-\alpha\\-\alpha&\alpha\end{pmatrix}.
$$

The [generalized eigenvalue problem for small oscillations](generalized-eigenvalue-problem-for-small-oscillations.md) is $Ka=\omega^2Ma$, not $Ka=m\omega^2a$. In particular the lower [Euler-Lagrange equation](euler-lagrange-equation.md) is $\ddot x_2=-(g/l)(x_2-x_1)$, independent of the lower mass factor after division by that [mass](mass.md). This reproduces the [normal modes of a double pendulum](normal-modes-of-a-double-pendulum.md) and distinguishes the [mechanical mass matrix](mechanical-mass-matrix.md) from its [stiffness matrix](stiffness-matrix.md).

## ↑ Ancestors (8)

1. [Normal modes of a double pendulum](normal-modes-of-a-double-pendulum.md)
2. [Generalized eigenvalue problem for small oscillations](generalized-eigenvalue-problem-for-small-oscillations.md)
3. [Small oscillation](small-oscillation.md)
4. [Lagrangian mechanics](lagrangian-mechanics-split.md)
5. [Classical mechanics](classical-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematical-methods-ii-course-of-the-university-of-oxford/2022/11/a/solution.md)
