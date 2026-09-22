<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

A [Hermitian operator](../../../../../hermitian-operator.md) $A$ satisfies $\langle\varphi,A\psi\rangle=\langle A\varphi,\psi\rangle$ on its [operator domain](../../../../../operator-domain.md). Here

$$
H=-\frac{\hbar^2}{2m}\frac{d^2}{dx^2}+V(x).
$$

Two [integration by parts](../../../../../integration-by-parts.md) operations, together with the boundary conditions in the Hamiltonian domain, show that the kinetic term is Hermitian; multiplication by the real function $V$ is Hermitian as well. Thus $H$ is Hermitian.

For a time-independent operator $A$, the [Schrödinger equation](../../../../../schrodinger-equation.md) and its adjoint give the [Ehrenfest theorem](../../../../../ehrenfest-theorem.md)

$$
\frac d{dt}\langle A\rangle=\frac{i}{\hbar}\langle[H,A]\rangle.
$$

Using the [canonical commutation relation](../../../../../canonical-commutation-relation.md) $[x,p]=i\hbar$,

$$
[H,x]=-\frac{i\hbar}{m}p,
\qquad
[H,p]=i\hbar V'(x).
$$

Consequently

$$
\boxed{\frac d{dt}\langle x\rangle=\frac1m\langle p\rangle,
\qquad
\frac d{dt}\langle p\rangle=-\langle V'(x)\rangle.}
$$

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
