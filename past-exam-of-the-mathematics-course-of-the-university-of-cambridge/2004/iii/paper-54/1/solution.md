<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

By the [Schmidt decomposition theorem](../../../../../schmidt-decomposition.md), suitable [local unitary operations](../../../../../local-unitary-operation.md) put the normalized [pure state](../../../../../pure-state.md) into the form

$$
|\psi\rangle=\lambda_0|00\rangle+\lambda_1|11\rangle,\qquad \lambda_0,\lambda_1\geq0,\qquad \lambda_0^2+\lambda_1^2=1.
$$

It is [entangled](../../../../../entangled-state.md) precisely when both [Schmidt coefficients](../../../../../schmidt-coefficient.md) are nonzero. Put $s=2\lambda_0\lambda_1$, so $0<s\leq1$ for the case of interest. The [Pauli operators](../../../../../pauli-operator.md)

$$
Z=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad X=\begin{pmatrix}0&1\\1&0\end{pmatrix}
$$

satisfy $\langle Z\otimes Z\rangle=1$ and $\langle X\otimes X\rangle=s$ in this [pure state](../../../../../pure-state.md): $Z\otimes Z$ fixes both basis terms, and $X\otimes X$ exchanges them.

Choose Alice's two [observables](../../../../../observable.md) as $A_0=Z$, $A_1=X$, and Bob's as

$$
B_0=\frac{Z+sX}{\sqrt{1+s^2}},\qquad B_1=\frac{Z-sX}{\sqrt{1+s^2}}.
$$

These are valid dichotomic [projective measurements](../../../../../projective-measurement.md). Indeed, $XZ+ZX=0$ and $X^2=Z^2=I$, so $B_0^2=B_1^2=I$; each [observable](../../../../../observable.md) has outcomes $\pm1$. For the [CHSH inequality](../../../../../chsh-inequality.md) convention $|\langle A_0\otimes(B_0+B_1)+A_1\otimes(B_0-B_1)\rangle|\leq2$, the quantum value is

$$
\begin{aligned}
S&=\frac{2}{\sqrt{1+s^2}}\big(\langle Z\otimes Z\rangle+s\langle X\otimes X\rangle\big)\\
&=\boxed{2\sqrt{1+s^2}>2.}
\end{aligned}
$$

For the original [pure state](../../../../../pure-state.md), conjugate these four [observables](../../../../../observable.md) by the corresponding local [unitary operators](../../../../../unitary-operator.md). Their outcomes and [Pauli correlators](../../../../../pauli-correlator.md) are unchanged, and each party still measures only their own [qubit](../../../../../qubit.md). Thus **every entangled pure two-qubit state violates CHSH for suitable local measurements**, proving [Gisin's theorem](../../../../../gisin-s-theorem.md) directly. The [CHSH axes for an entangled pure two-qubit state](../../../../../chsh-axes-for-an-entangled-pure-two-qubit-state.md) approach a nonviolating configuration continuously as one [Schmidt coefficient](../../../../../schmidt-coefficient.md) tends to zero; the strict violation therefore need not be large for weak [entanglement](../../../../../entangled-state.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
