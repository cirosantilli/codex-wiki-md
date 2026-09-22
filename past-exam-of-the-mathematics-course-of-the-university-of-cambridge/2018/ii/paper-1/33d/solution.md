<h1 id="33d/solution">Solution</h1>

↑ **Parent:** [33D](../33d.md)

From the [creation and annihilation operators](../../../../../creation-and-annihilation-operators.md) commutator,

$$
[H,A]=\hbar\omega[A^\dagger A,A]=-\hbar\omega A.
$$

Therefore $A|n\rangle$ is either zero or an [energy eigenstate](../../../../../energy-eigenstate.md) with energy $E_n-\hbar\omega=E_{n-1}$. Since each energy level of the one-dimensional [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md) is [nondegenerate](../../../../../nondegenerate-bilinear-form.md), $A|n\rangle=c_n|n-1\rangle$. Its [norm](../../../../../norm.md) determines the coefficient:

$$
|c_n|^2=\langle n|A^\dagger A|n\rangle=n.
$$

Choosing the conventional phases of the [number states](../../../../../number-state.md) gives

$$
\boxed{A|n\rangle=\sqrt n\,|n-1\rangle.}
$$

Solving the given relation for the [position operator](../../../../../position-operator.md) gives

$$
X=\sqrt{\frac{\hbar}{2m\omega}}(A+A^\dagger).
$$

Put $Q=A+A^\dagger$. Repeated use of the ladder relations gives

$$
Q|0\rangle=|1\rangle,
\qquad Q^2|0\rangle=|0\rangle+\sqrt2|2\rangle,
$$



$$
Q^3|0\rangle=3|1\rangle+\sqrt6|3\rangle,
\qquad
Q^4|0\rangle=3|0\rangle+6\sqrt2|2\rangle+2\sqrt6|4\rangle.
$$

Hence

$$
X^4|0\rangle=\left(\frac{\hbar}{2m\omega}\right)^2
\left(3|0\rangle+6\sqrt2|2\rangle+2\sqrt6|4\rangle\right).
$$

In [first-order nondegenerate perturbation theory](../../../../../first-order-nondegenerate-perturbation-theory.md), the $|0\rangle$ component is omitted from the state correction, while $E_0-E_2=-2\hbar\omega$ and $E_0-E_4=-4\hbar\omega$. It follows that

$$
\boxed{|0_\lambda\rangle
=|0\rangle-\frac{\hbar\lambda}{4m^2\omega^3}
\left(3\sqrt2|2\rangle+\sqrt{\frac32}|4\rangle\right)+O(\lambda^2),}
$$

which is the [first-order ground state of the quartic oscillator](../../../../../first-order-ground-state-of-the-quartic-oscillator.md).

## ↑ Ancestors (10)

1. [33D](../33d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
