<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take a [normalized](../../../../normalization.md) vector in the required common [operator domains](../../../../operator-domain.md). Expanding the squared [norm](../../../../norm.md) and using [self-adjointness](../../../../self-adjoint-operator.md) gives

$$
\|(A-itB)\psi\|^2=\langle\psi,(A+itB)(A-itB)\psi\rangle=\langle A^2\rangle+t^2\langle B^2\rangle-it\langle[A,B]\rangle.
$$

Thus its final term is $\hbar t\langle C\rangle$. Set $a=\|A\psi\|^2$, $b=\|B\psi\|^2$, $c=\langle C\rangle$. If $b>0$, minimizing the nonnegative quadratic at $t_*=-\hbar c/(2b)$ gives

$$
\boxed{4ab\geq\hbar^2c^2.}
$$

Equality holds precisely when the minimum [norm](../../../../norm.md) vanishes, that is $(A-it_*B)\psi=0$. If $b=0$, however, then $B\psi=0$ and $c=0$, so equality is automatic [even](../../../../even-function.md) when $A\psi\ne0$. **The printed equality criterion needs this zero-vector exception.** For example $A=I$, $B=0$, $C=0$ saturates the inequality but admits no such real $t$. The exact general criterion is [linear dependence](../../../../linear-dependence.md) of $A\psi,B\psi$ together with vanishing real part of their [inner product](../../../../inner-product-split.md), as in the [uncentered second-moment commutator inequality](../../../../uncentered-second-moment-commutator-inequality.md).

Apply the same calculation to $A-\langle A\rangle I$, $B-\langle B\rangle I$, whose [commutator](../../../../commutator.md) is unchanged. This gives the [Robertson uncertainty principle](../../../../robertson-uncertainty-principle.md)

$$
\boxed{4(\Delta A)^2(\Delta B)^2\geq\hbar^2\langle C\rangle^2.}
$$

If $\psi$ is an [eigenvector](../../../../eigenvector.md) of $A$, its [dispersion](../../../../wave-dispersion.md) is zero; finite [dispersion](../../../../wave-dispersion.md) of $B$ then forces $\boxed{\langle C\rangle=0}$.

In the [position representation](../../../../position-representation-in-quantum-mechanics.md), $X\psi=x\psi$ and $P\psi=-i\hbar\psi'$. The [product rule](../../../../product-rule.md) gives $[P,X]\psi=-i\hbar\psi$, hence $\boxed{[P,X]=-i\hbar I}$. Since $V(X)$ commutes with $X$,

$$
\boxed{[H,X]=\frac1{2m}\{P[P,X]+[P,X]P\}=-\frac{i\hbar}{m}P.}
$$

For an [energy eigenstate](../../../../energy-eigenstate.md), $\langle[H,X]\rangle=E\langle X\rangle-E\langle X\rangle=0$, so $\boxed{\langle P\rangle=0}$. For the oscillator $[H,P]=i\hbar m\omega^2X$, and the same argument gives $\boxed{\langle X\rangle=0}$. These [expectation](../../../../expected-value-split.md) identities require the stated finite moments and [commutator](../../../../commutator.md) domains; formal position [eigenvectors](../../../../eigenvector.md) are not normalizable exceptions.

Apply the [Robertson uncertainty principle](../../../../robertson-uncertainty-principle.md) to each angular-momentum pair:

$$
\boxed{4(\Delta L_1)^2(\Delta L_2)^2\geq\hbar^2\langle L_3\rangle^2.}
$$

If $\psi$ is an [eigenvector](../../../../eigenvector.md) of $L_3$, then $\Delta L_3=0$. The inequalities for $(L_2,L_3)$ and $(L_3,L_1)$ force $\boxed{\langle L_1\rangle=\langle L_2\rangle=0}$, assuming the relevant moments exist.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
