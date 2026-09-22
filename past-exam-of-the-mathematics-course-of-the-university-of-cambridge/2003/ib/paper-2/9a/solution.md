<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

A [Hermitian operator](../../../../../hermitian-operator.md) satisfies $\langle u,Av\rangle=\langle Au,v\rangle$ for all admissible states in its domain; in finite dimension this is $A^*=A$. For an unbounded physical observable one specifies a self-adjoint realization, rather than only a formal differential expression.

Here $p=-i\hbar\,d/dx$ and $H=-\hbar^2d^2/(2m\,dx^2)+V(x)$. For states with sufficient regularity and decay, integration by parts gives

$$
\langle u,Hv\rangle-\langle Hu,v\rangle
=-\frac{\hbar^2}{2m}[\bar u v'-\bar u'v]_{-\infty}^{\infty}=0.
$$

The multiplication term cancels because $V$ is real. Thus the [Quantum Hamiltonian](../../../../../hamiltonian-quantum-mechanics.md) is Hermitian on the stated admissible domain. Equivalent boundary conditions must remove this boundary term if the system is on a bounded interval.

The [Schrödinger equation](../../../../../schrodinger-equation.md) $i\hbar\dot\psi=H\psi$ and its conjugate imply, for a time-independent observable $A$ and normalized state,

$$
\frac d{dt}\langle A\rangle
=\frac i\hbar\langle HA-AH\rangle.
$$

This follows by differentiating both factors in $\langle\psi,A\psi\rangle$ and moving $H$ using Hermiticity. The canonical [commutator](../../../../../commutator.md) $[x,p]=i\hbar$ gives

$$
[H,x]=-\frac{i\hbar}{m}p,\qquad [H,p]=[V,p]=i\hbar V'(x).
$$

Consequently the two [Ehrenfest theorem](../../../../../ehrenfest-theorem.md) identities are

$$
\boxed{\frac d{dt}\langle x\rangle=\frac{\langle p\rangle}{m},\qquad
\frac d{dt}\langle p\rangle=-\langle V'(x)\rangle.}
$$

They require the displayed expectations and domain operations to exist; real-valuedness of a potential alone is not a proof about every possible singular operator domain.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
