<h1 id="7g/solution">Solution</h1>

↑ **Parent:** [7G](../7g.md)

For a state in the domain of the operator, its [expectation value](../../../../../expectation-value.md) is

$$
\langle\mathcal O\rangle=\frac{\int\Psi^*(x,t)(\mathcal O\Psi)(x,t)\,dx}{\int|\Psi(x,t)|^2dx}.
$$

For a normalized state the denominator is one. Use an orthonormal [energy eigenstate](../../../../../energy-eigenstate.md) basis, choosing orthogonal vectors within degenerate eigenspaces. Inserting an expansion into the time-dependent [Schrödinger equation](../../../../../schrodinger-equation.md) gives $i\hbar\dot a_n(t)=E_na_n(t)$. Consequently

$$
\boxed{\Psi(x,t)=\sum_n a_n e^{-iE_nt/\hbar}u_n(x)}.
$$

The phases preserve normalization. Projection onto a specified basis eigenstate gives probability $\boxed{|a_p|^2}$, independent of time. If the measurement distinguishes only the energy and $E_p$ is degenerate, sum $|a_n|^2$ over all $n$ with $E_n=E_p$.

Using orthonormality to eliminate all cross terms,

$$
\boxed{\langle H\rangle=\sum_n|a_n|^2E_n}.
$$

This is time independent whenever the expectation is defined. The time-independent Hamiltonian changes only relative phases, not the energy probabilities.

## ↑ Ancestors (10)

1. [7G](../7g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
