<h1 id="8e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First consider rotation predominantly about the third [principal axis](../../../../../../principal-axis.md), writing $\omega_3=\Omega+O(\omega_1^2+\omega_2^2)$. To first order the third Euler equation gives $\dot\Omega=0$, while the transverse components satisfy

$$
\dot\omega_1=\frac{I_2-I_3}{I_1}\Omega\omega_2,
\qquad
\dot\omega_2=\frac{I_3-I_1}{I_2}\Omega\omega_1.
$$

Therefore

$$
\ddot\omega_1
=-\Omega^2\frac{(I_3-I_2)(I_3-I_1)}{I_1I_2}\omega_1,
$$

and the same equation holds for $\omega_2$.

Order the principal moments as $I_1<I_2<I_3$. The coefficient above is negative, so perturbations about axis three oscillate and remain bounded. Cyclically applying the same [linear stability of principal-axis rotation](../../../../../../linear-stability-of-principal-axis-rotation.md) calculation about axis one gives

$$
\ddot\omega_2
=-\Omega^2\frac{(I_2-I_1)(I_3-I_1)}{I_2I_3}\omega_2,
$$

so that rotation is also stable. About axis two, however,

$$
\ddot\omega_1
=+\Omega^2\frac{(I_2-I_1)(I_3-I_2)}{I_1I_3}\omega_1,
$$

which has an exponentially growing solution. Thus the [intermediate axis theorem](../../../../../../intermediate-axis-theorem.md) gives

$$
\boxed{\text{rotation about the smallest and largest inertia axes is stable, while rotation about the intermediate axis is unstable.}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
