<h1 id="15b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Subtracting $I_2$ times the energy identity from the angular-momentum identity, under $L^2=2EI_2$, gives

$$
I_1(I_2-I_1)\omega_1^2
=I_3(I_3-I_2)\omega_3^2.
$$

Combining this with

$$
I_1\omega_1^2+I_3\omega_3^2
=2E-I_2\omega_2^2
=\frac{L^2}{I_2}-I_2\omega_2^2
$$

yields

$$
\omega_1^2=
\frac{I_3-I_2}{I_1(I_3-I_1)}
\left(2E-I_2\omega_2^2\right)
$$

and

$$
\omega_3^2=
\frac{I_2-I_1}{I_3(I_3-I_1)}
\left(2E-I_2\omega_2^2\right).
$$

The second Euler equation now gives, after squaring or choosing one orientation of the orbit,

$$
\dot\omega_2
=\pm\sqrt{\frac{(I_3-I_2)(I_2-I_1)}{I_1I_3}}
\left(\mu^2-\omega_2^2\right),
\qquad
\mu=\sqrt{\frac{2E}{I_2}}.
$$

Indeed, the factor $I_3-I_1$ in $I_2\dot\omega_2=(I_3-I_1)\omega_3\omega_1$ cancels the denominator from the product of the two preceding expressions.

For the plus sign, separation gives

$$
\operatorname{artanh}\frac{\omega_2}{\mu}
=\mu\sqrt{\frac{(I_3-I_2)(I_2-I_1)}{I_1I_3}}\,(t-t_0).
$$

After choosing the time origin $t_0=0$,

$$
\boxed{\omega_2(t)=\mu\tanh(\lambda t)},
\qquad
\boxed{\lambda=\mu
\sqrt{\frac{(I_3-I_2)(I_2-I_1)}{I_1I_3}}}.
$$

For example, a compatible choice of the other components is

$$
\omega_1(t)=
\sqrt{\frac{2E(I_3-I_2)}{I_1(I_3-I_1)}}\operatorname{sech}(\lambda t),
$$



$$
\omega_3(t)=
\sqrt{\frac{2E(I_2-I_1)}{I_3(I_3-I_1)}}\operatorname{sech}(\lambda t).
$$

As $t$ runs from $-\infty$ to $+\infty$, the solution approaches the rotations $\omega_2=-\mu$ and $\omega_2=+\mu$. It is the [intermediate-axis separatrix](../../../../../../intermediate-axis-separatrix.md), a heteroclinic trajectory that exhibits the instability found in part (b).

## ↑ Ancestors (11)

1. [C](../c.md)
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
