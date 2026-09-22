# Transition frequencies and matrix multiplication

↑ **Parent:** [Observable matrices in an energy basis](observable-matrices-in-an-energy-basis.md)

In the [Heisenberg picture](heisenberg-picture.md), an [observable](observable.md) without explicit time dependence has

$$
A_H(t)=e^{iHt/\hbar}Ae^{-iHt/\hbar},\qquad (A_H)_{mn}(t)=A_{mn}e^{i\omega_{mn}t},\qquad \omega_{mn}=\frac{E_m-E_n}{\hbar}.
$$

Here $\hbar$ is the reduced [Planck constant](planck-constant.md). An emitted [photon](photon.md) on a transition $n\to m$ with $E_n>E_m$ has positive [angular frequency](angular-frequency.md) $(E_n-E_m)/\hbar=|\omega_{mn}|$. The sign of the array's [quantum phase](quantum-phase.md) follows its index convention; it is not a negative measured [photon](photon.md) [frequency](frequency.md). The frequencies involve differences of [energy levels](energy-level.md), rather than the absolute values $E_n/\hbar$. Adding a constant to $H$ leaves these frequencies unchanged.

Insert the complete [orthonormal basis](orthonormal-basis.md) between two [linear operators](linear-operator.md):

$$
(AB)_{mn}=\sum_k A_{mk}B_{kn},\qquad \omega_{mk}+\omega_{kn}=\omega_{mn}.
$$

The sum runs over intermediate states. The second identity follows by cancellation of $E_k$; it makes every term in the product acquire the same time factor $e^{i\omega_{mn}t}$. This is a useful reason for [matrix multiplication](matrix-multiplication.md): it composes the two indexed arrays consistently with the addition of transition frequencies. It does not multiply matching entries independently. Swapping $A$ and $B$ generally changes the intermediate-state sum and hence the result.

## ↑ Ancestors (7)

1. [Observable matrices in an energy basis](observable-matrices-in-an-energy-basis.md)
2. [Matrix mechanics](matrix-mechanics.md)
3. [Operator formalism](operator-formalism.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
