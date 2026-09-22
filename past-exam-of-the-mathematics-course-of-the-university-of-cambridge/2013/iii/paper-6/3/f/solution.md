<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [orthogonal projection](../../../../../../orthogonal-projection.md) satisfies $\Pi L=\Pi(\Pi-I)=0$, hence $d\Pi f_t/dt=0$ and $\Pi f_t=\Pi f_0=\rho(f_0)M$. Set $h_t=f_t-\Pi f_0$. Then $\Pi h_t=0$ and $\dot h_t=Lh_t$. Crucially, applying the energy identity of part (e) to $h_t$ gives

$$
\frac{d}{dt}\|h_t\|_H^2=2\operatorname{Re}\langle Lh_t,h_t\rangle=-2\|h_t-\Pi h_t\|_H^2=-2\|h_t\|_H^2.
$$

Solving this scalar equation and taking square roots proves

$$
\boxed{\|f_t-\rho(f_0)M\|_H=e^{-t}\|f_0-\rho(f_0)M\|_H}.
$$

This argument uses (e) explicitly, rather than bypassing the requested [energy method](../../../../../../energy-method.md) with an explicit solution formula.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
