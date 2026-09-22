<h1 id="11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First solve the supplied equations as a linear system, with $\omega_0^2=g/l$ and $\alpha>0$. A [normal mode](../../../../normal-mode.md) $\mathbf x=\mathbf a e^{i\omega t}$ obeys

$$
\frac{\omega^2}{\omega_0^2}\mathbf a=D\mathbf a,\qquad
D=\begin{pmatrix}1+2\alpha&-\alpha\\-\alpha&\alpha\end{pmatrix}.
$$

Its [characteristic polynomial](../../../../characteristic-polynomial.md) is $\lambda^2-(1+3\alpha)\lambda+\alpha(1+\alpha)$. Hence

$$
\boxed{\omega_\pm^2=\frac g{2l}\left[1+3\alpha\pm\sqrt{1+2\alpha+5\alpha^2}\right].}
$$

Both are positive, since the [trace](../../../../matrix-trace.md) and [determinant](../../../../determinant.md) of $D$ are positive.

There is a physical discrepancy in the source. The [horizontal-coordinate mass matrix of an unequal-mass double pendulum](../../../../horizontal-coordinate-mass-matrix-of-an-unequal-mass-double-pendulum.md) follows from the stated horizontal [displacements](../../../../displacement.md), which give

$$
T_2=\frac m2\dot x_1^2+\frac{\alpha m}{2}\dot x_2^2,\qquad
V_2=\frac{mg}{2l}\left[x_1^2+\alpha x_1^2+\alpha(x_2-x_1)^2\right].
$$

The [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) reproduce the supplied upper equation, but give $\ddot x_2=-(g/l)(x_2-x_1)$, without its extra $\alpha$. The true [normal modes of a double pendulum](../../../../normal-modes-of-a-double-pendulum.md) consequently have $\omega_\pm^2=(g/l)[1+\alpha\pm\sqrt{\alpha(1+\alpha)}]$. The boxed answer and the remaining parts below concern the explicitly supplied linear system. The two models agree at $\alpha=1$, but not for a general mass ratio.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [11](../../11.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
