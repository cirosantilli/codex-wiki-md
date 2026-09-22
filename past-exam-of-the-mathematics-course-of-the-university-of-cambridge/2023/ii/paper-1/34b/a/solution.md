<h1 id="34b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In units with $\hbar=1$, the [quantum harmonic oscillator](../../../../../../quantum-harmonic-oscillator.md) Hamiltonian and [number operator](../../../../../../number-operator.md) are

$$
\boxed{H=\omega\left(N+\frac12\right)},
\qquad
\boxed{N=A^\dagger A}.
$$

The nontrivial commutators among the [creation and annihilation operators](../../../../../../creation-and-annihilation-operators.md) and $N$ are

$$
\boxed{
[A,A^\dagger]=1,
\qquad
[N,A]=-A,
\qquad
[N,A^\dagger]=A^\dagger
}.
$$

Their reversed commutators have the opposite signs, while the commutator of any operator with itself is zero.

The operator $N$ is [self-adjoint](../../../../../../self-adjoint-operator.md) because

$$
(A^\dagger A)^\dagger=A^\dagger A.
$$

Its eigenvalues are therefore real. Moreover, for every state $|\psi\rangle$,

$$
\langle\psi|N|\psi\rangle
=\langle A\psi|A\psi\rangle
=\|A|\psi\rangle\|^2\geq0,
$$

so every eigenvalue is nonnegative.

If $N|\nu\rangle=\nu|\nu\rangle$, the commutator with $A$ gives

$$
N(A|\nu\rangle)=(\nu-1)A|\nu\rangle,
$$

and

$$
\|A|\nu\rangle\|^2=\nu\|\,|\nu\rangle\|^2.
$$

Repeated application of $A$ lowers the eigenvalue by one. It must terminate before producing a negative eigenvalue. If $m$ is the last occupied rung, then $A|\nu-m\rangle=0$, and the norm identity forces $\nu-m=0$. Hence

$$
\boxed{\nu\in\{0,1,2,\ldots\}}.
$$

This is the [integer spectrum of the number operator](../../../../../../integer-spectrum-of-the-number-operator.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [34B](../../34b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
