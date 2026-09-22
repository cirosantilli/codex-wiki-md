<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

Let the heavier block move downward, so no slip gives linear acceleration $a\dot\omega$. Newton's equations and the pulley [torque](../../../../../torque.md) equation are

$$
T_1-Mg=Ma\dot\omega,\qquad
2Mg-T_2=2Ma\dot\omega,
$$



$$
(T_2-T_1)a-\lambda M\omega=qMa^2\dot\omega.
$$

Eliminating the tensions gives the first-order equation

$$
\boxed{(q+3)a^2\dot\omega+\lambda\omega=ga}.
$$

With $\omega(0)=0$, its solution is

$$
\boxed{\omega(t)=\frac{ga}{\lambda}
\left(1-e^{-\lambda t/[(q+3)a^2]}\right)}.
$$

For a thin slice of the solid of revolution, $dM=\rho\pi b(x)^2dx$ and its axial [moment of inertia](../../../../../moment-of-inertia.md) is $dI=\tfrac12b(x)^2dM$. Consequently

$$
q=\frac{I}{Ma^2}
=\frac12\frac{\int_{-1}^1(1+|x|)^4dx}
{\int_{-1}^1(1+|x|)^2dx}
=\frac12\frac{62/5}{14/3}
=\boxed{\frac{93}{70}}.
$$

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
