<h1 id="14c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a normalized wavefunction obeying the infinite-wall [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md), integration by parts gives the energy expectation

$$
\langle H\rangle
=\int_0^a\left(\frac{\hbar^2}{2m}|\psi'(x)|^2
+U(x)|\psi(x)|^2\right)\,dx\geq0.
$$

Thus every [energy eigenvalue](../../../../../../energy-eigenvalue.md) is nonnegative.

For $0<E<U_0$, the [Time-independent Schrödinger equation](../../../../../../time-independent-schrodinger-equation.md) and the wall conditions give

$$
\psi(x)=
\begin{cases}
A\sin(kx),&0\leq x\leq a/2,\\
B\sinh(l(a-x)),&a/2\leq x\leq a,
\end{cases}
$$

where $k=\sqrt{2mE}/\hbar$ and $l=\sqrt{2m(U_0-E)}/\hbar$. Continuity of $\psi$ and $\psi'$ at the finite potential step gives

$$
A\sin(ka/2)=B\sinh(la/2),
$$



$$
Ak\cos(ka/2)=-Bl\cosh(la/2).
$$

Dividing and rearranging yields the [bound-state quantization condition](../../../../../../bound-state-quantization-condition.md)

$$
\boxed{\frac1k\tan\frac{ka}{2}
=-\frac1l\tanh\frac{la}{2}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [14C](../../14c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
