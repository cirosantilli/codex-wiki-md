<h1 id="8e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $e_1,e_2,e_3$ be a [principal body frame](../../../../../../principal-body-frame.md), let $I_1,I_2,I_3$ be the corresponding principal [moments of inertia](../../../../../../moment-of-inertia.md), and write the [angular velocity](../../../../../../angular-velocity.md) as $\boldsymbol\omega=\sum_i\omega_i e_i$. The body-frame components of the [angular momentum](../../../../../../angular-momentum.md) are

$$
\mathbf L=\sum_{i=1}^3 I_i\omega_i e_i.
$$

No external torque acts, so $\mathbf L$ is constant in the [fixed space frame](../../../../../../fixed-space-frame.md). Since a body-fixed basis vector satisfies $\dot e_i=\boldsymbol\omega\times e_i$,

$$
0=\left(\frac{d\mathbf L}{dt}\right)_{\rm space}
=\left(\frac{d\mathbf L}{dt}\right)_{\rm body}
+\boldsymbol\omega\times\mathbf L.
$$

Taking body-frame components gives the [Euler equations for a torque-free rigid body](../../../../../../euler-equations-for-a-torque-free-rigid-body.md):

$$
\boxed{
\begin{aligned}
I_1\dot\omega_1&=(I_2-I_3)\omega_2\omega_3,\\
I_2\dot\omega_2&=(I_3-I_1)\omega_3\omega_1,\\
I_3\dot\omega_3&=(I_1-I_2)\omega_1\omega_2.
\end{aligned}}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
