<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $a=R/(2L)$ and $\omega_d=\sqrt{1/(LC)-a^2}>0$. The roots of the [characteristic polynomial](../../../characteristic-polynomial.md) are $-a\pm i\omega_d$, so the real underdamped solution is $Q=e^{-at}(A\cos\omega_dt+B\sin\omega_dt)$. The initial charge gives $A=Q_0$ and the zero initial current gives $B=aQ_0/\omega_d$. Hence

$$
\boxed{Q(t)=Q_0e^{-Rt/(2L)}\left[\cos(\omega_dt)+\frac{R}{2L\omega_d}\sin(\omega_dt)\right].}
$$

This solves the homogeneous [RLC circuit](../../../rlc-circuit.md) equation supplied in the question. A nonzero applied voltage would appear as a forcing term and require a particular solution; it is not present in that equation.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2022](../../2022-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
