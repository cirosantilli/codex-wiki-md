<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The fixed-particle-number sector is spanned by $|1\rangle=c_1^\dagger|0\rangle$ and $|2\rangle=c_2^\dagger|0\rangle$. In this basis,

$$
H=-t\begin{pmatrix}0&1\\1&0\end{pmatrix}=-t\sigma_x.
$$

The relevant [quantum Gibbs state](../../../../quantum-gibbs-state.md) is normalized within this two-dimensional sector, not over all particle numbers. With $\beta=(k_BT)^{-1}$ and $x=\beta t$, the [exponential of a Pauli vector](../../../../exponential-of-a-pauli-vector.md) gives

$$
e^{-\beta H}=e^{x\sigma_x}=I\cosh x+\sigma_x\sinh x,\qquad
Z=2\cosh x.
$$

Therefore

$$
\boxed{\rho_\beta=\frac12(I+\tanh x\,\sigma_x)
=\frac12\begin{pmatrix}1&\tanh x\\\tanh x&1\end{pmatrix}}.
$$

Its [eigenstates](../../../../eigenstate.md) are $|\pm\rangle=(|1\rangle\pm|2\rangle)/\sqrt2$, with energies $\mp t$ and probabilities $p_\pm=e^{\pm x}/(2\cosh x)$. These are nonnegative and sum to one, so the [matrix](../../../../matrix.md) is [Hermitian](../../../../hermitian-operator.md) and has [trace](../../../../matrix-trace.md) one. Its [purity of a density operator](../../../../purity-of-a-density-operator.md) is

$$
\boxed{\operatorname{Tr}\rho_\beta^2=\frac12(1+\tanh^2x)}.
$$

For $t\ne0$, the zero-temperature limit is the pure ground-state projector,

$$
\rho_{T\to0}=\frac12[I+\operatorname{sgn}(t)\sigma_x],
$$

with purity one. As $T\to\infty$, $x\to0$ and $\rho\to I/2$, with purity $1/2$. At every strictly positive finite [temperature](../../../../temperature-split.md) and finite $t$, both [eigenvalues](../../../../eigenvalue.md) are nonzero, so the state is mixed. If $t=0$, the two levels are degenerate and the Gibbs state is $I/2$ at all temperatures, including its zero-temperature limit.

Using [dimensionless](../../../../dimensionless-quantity.md) [Von Neumann entropy](../../../../von-neumann-entropy-split.md), $S=-\operatorname{Tr}(\rho\ln\rho)$, gives

$$
\boxed{S(T)=-p_+\ln p_+-p_-\ln p_-
=\ln(2\cosh x)-x\tanh x}.
$$

For nonzero $t$, $S\to0$ as $T\to0$, while $S\to\ln2$ as $T\to\infty$. More precisely, the high-temperature expansion is $S=\ln2-x^2/2+O(x^4)$, and the low-temperature form is $S\sim(1+2|x|)e^{-2|x|}$. The thermodynamic entropy includes an overall factor $k_B$.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
