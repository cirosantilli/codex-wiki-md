<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a vector $\mathbf A=\sum_i A_i\mathbf e_i$ in the [principal body frame](../../../../../principal-body-frame.md), the [derivative of a body-fixed basis vector](../../../../../derivative-of-a-body-fixed-basis-vector.md) is $(d\mathbf e_i/dt)_{\widehat S}=\boldsymbol\omega\times\mathbf e_i$. Differentiating the expansion gives the [rotating-frame derivative formula](../../../../../rotating-frame-derivative-formula.md), also called the Coriolis formula:

$$
\left(\frac{d\mathbf A}{dt}\right)_{\widehat S}
=\left(\frac{d\mathbf A}{dt}\right)_S+\boldsymbol\omega\times\mathbf A.
$$

Apply this to [angular momentum](../../../../../angular-momentum.md) $\mathbf L=\sum_iI_i\omega_i\mathbf e_i$. The [principal moments of inertia](../../../../../principal-moment-of-inertia.md) are constant in the [principal body frame](../../../../../principal-body-frame.md), so external [torque](../../../../../torque.md) balance becomes

$$
\boldsymbol\tau=\mathbf I\dot{\boldsymbol\omega}+\boldsymbol\omega\times(\mathbf I\boldsymbol\omega).
$$

Resolving the [cross product](../../../../../cross-product.md) gives [Euler's equations](../../../../../euler-s-equations-rigid-body-dynamics.md):

$$
\boxed{\begin{aligned}
I_1\dot\omega_1+(I_3-I_2)\omega_2\omega_3&=\tau_1,\\
I_2\dot\omega_2+(I_1-I_3)\omega_3\omega_1&=\tau_2,\\
I_3\dot\omega_3+(I_2-I_1)\omega_1\omega_2&=\tau_3.
\end{aligned}}
$$

All components and dotted components in this display refer to the [principal body frame](../../../../../principal-body-frame.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the classical mechanics course of the University of Oxford](../../../../split.md)
6. [Classical mechanics course of the University of Oxford](../../../../../classical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
