<h1 id="15b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Setting $\omega_1=\omega_3=0$ makes all three Euler equations stationary. The invariants then give

$$
E=\frac12I_2\omega_2^2,
\qquad
L^2=I_2^2\omega_2^2=2EI_2,
$$

so the two rotations are

$$
\omega_2=\pm\sqrt{\frac{2E}{I_2}}
=\pm\frac{L}{I_2},
$$

where $L=\sqrt{L^2}$.

Linearize about $(0,\Omega,0)$, where $\Omega$ is either of these values. Writing the transverse perturbations as $(\xi,\zeta)=(\delta\omega_1,\delta\omega_3)$ gives

$$
I_1\dot\xi=(I_2-I_3)\Omega\zeta,
\qquad
I_3\dot\zeta=(I_1-I_2)\Omega\xi.
$$

Consequently

$$
\ddot\xi
=\Omega^2\frac{(I_3-I_2)(I_2-I_1)}{I_1I_3}\,\xi.
$$

The transverse eigenvalues are therefore

$$
s=\pm |\Omega|
\sqrt{\frac{(I_3-I_2)(I_2-I_1)}{I_1I_3}},
$$

one of which is positive. Both rotations are linearly unstable, which is the [intermediate axis theorem](../../../../../../intermediate-axis-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15B](../../15b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
