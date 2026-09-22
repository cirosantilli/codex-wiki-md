<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [density operator](../../../../density-matrix-split.md) is a positive self-adjoint trace-class operator with trace one. In finite dimensions this is a positive semidefinite [Hermitian matrix](../../../../hermitian-operator.md) with $\operatorname{tr}\rho=1$. Its expectation of an observable is $\boxed{\langle A\rangle=\operatorname{tr}(A\rho)}$ whenever the expectation is defined.

In the source's square-root notation, take the unique positive square root $W=\sqrt\rho$. It has Hilbert-Schmidt [norm](../../../../norm.md) one and satisfies $WW^*=\rho$, so

$$
\boxed{\operatorname{tr}(A\rho)=\operatorname{tr}(W^*AW).}
$$

The standard vector [purification](../../../../purification-of-a-density-operator.md) is the associated vector $|W\rangle\!\rangle=\sum_{r,s}W_{rs}|\xi_r\rangle|\eta_s\rangle$ on a system and a chosen copy. Tracing out the copy gives $\rho$; measuring $A\otimes I$ gives the same trace formula. Thus the operator square root and the purified vector are two related objects, distinguished by this vectorization.

For a general coefficient matrix $C$, expansion of the expectation gives

$$
\langle\Psi|A\otimes I|\Psi\rangle
=\sum_{r,t,s}\overline{c_{rs}}A_{rt}c_{ts}
=\operatorname{tr}(ACC^*).
$$

Thus $\boxed{\rho_1=CC^*}$. Positivity is immediate from $v^*CC^*v=\|C^*v\|^2$, and its trace is one by [normalization](../../../../normalization.md) of $\Psi$.

If $C$ is nonsingular, it is square and $\rho_1$ is positive definite. Define

$$
\boxed{U=C^{-1}\sqrt{\rho_1}.}
$$

Then $UU^*=C^{-1}\rho_1(C^*)^{-1}=I$, which for a square matrix also implies $U^*U=I$. Thus $U$ is unitary, $\sqrt{\rho_1}=CU$, and $C=\sqrt{\rho_1}U^*$.

In an eigenbasis of $\rho_1$, its square root is $\operatorname{diag}(\sqrt{p_r})$. Hence $c_{rs}=\sqrt{p_r}\,\overline{U_{sr}}$. Define

$$
\boxed{|\zeta_r\rangle=\sum_s\overline{U_{sr}}|\eta_s\rangle.}
$$

Unitarity gives $\langle\zeta_r|\zeta_t\rangle=\delta_{rt}$, and substitution gives the [Schmidt decomposition](../../../../schmidt-decomposition.md)

$$
\boxed{|\Psi\rangle=\sum_r\sqrt{p_r}|\xi_r\rangle|\zeta_r\rangle.}
$$

For singular or rectangular $C$, the same conclusion follows on its support by a [singular value decomposition](../../../../singular-value-decomposition.md); the stated nonsingular case needs only the unitary calculation above.

For the supplied [Bell state](../../../../bell-state-split.md), the requested matrices are

$$
\boxed{C=\frac1{\sqrt2}\begin{pmatrix}0&1\\-1&0\end{pmatrix},\quad
\rho_1=\frac12I,\quad\sqrt{\rho_1}=\frac1{\sqrt2}I,\quad
U=\begin{pmatrix}0&-1\\1&0\end{pmatrix}.}
$$

The Schmidt vectors can be chosen as $\zeta_1=\eta_2$, $\zeta_2=-\eta_1$, and the two coefficients are $1/\sqrt2$. The square root's canonical vector [purification](../../../../purification-of-a-density-operator.md) is $(|\xi_1\eta_1\rangle+|\xi_2\eta_2\rangle)/\sqrt2$; the original Bell vector is a different [purification](../../../../purification-of-a-density-operator.md) of the same reduced state, related by a unitary on the second factor. This illustrates the unitary freedom of [purification](../../../../purification-of-a-density-operator.md).

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
