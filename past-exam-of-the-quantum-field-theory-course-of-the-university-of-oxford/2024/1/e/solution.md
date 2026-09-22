<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume $m_\psi>0$, as required to have a [rest frame](../../../../rest-frame.md). Choose the [Lorentz boost](../../../../lorentz-boost.md) $\Lambda$ for which $\Lambda p=(m_\psi,\mathbf0)$, and write its [unitary operator](../../../../unitary-operator.md) as $U$. The stipulated [one-particle state](../../../../one-particle-state.md) normalization gives $U|\psi,\mathbf p\rangle=|\psi,\mathbf0\rangle$ without a momentum-dependent prefactor. A [Lorentz scalar](../../../../lorentz-scalar.md) at the origin satisfies $U\phi(0)U^\dagger=\phi(0)$, and the [vacuum state](../../../../vacuum-state.md) satisfies $U|\Omega\rangle=|\Omega\rangle$. Inserting $U^\dagger U$ therefore proves

$$
\boxed{\langle\Omega|\phi(0)|\psi,\mathbf p\rangle=\langle\Omega|\phi(0)|\psi,\mathbf0\rangle.}
$$

With a noncovariant normalization of [momentum eigenstates](../../../../momentum-eigenstate.md), the assumed boost law would instead contain a square-root energy factor, so this equality is specifically tied to the paper's assumption.

Let $q^\mu=(E_{\mathbf q}^{\chi},\mathbf q)$ denote the [four-momentum](../../../../four-momentum.md) of the other [energy eigenstate](../../../../energy-eigenstate.md). Translation covariance first gives

$$
\langle\chi,\mathbf q|\phi(x)|\psi,\mathbf p\rangle
=e^{i(q-p)\cdot x}\langle\chi,\mathbf q|\phi(0)|\psi,\mathbf p\rangle
=e^{i(q-p)\cdot x}\langle U\chi,\mathbf q|\phi(0)|\psi,\mathbf0\rangle.
$$

Thus a suitable ket, including the phase whose complex conjugate appears in its bra, is

$$
\boxed{|\Psi\rangle=e^{-i(q-p)\cdot x}U|\chi,\mathbf q\rangle.}
$$

Here $\langle U\chi,\mathbf q|$ means $(U|\chi,\mathbf q\rangle)^\dagger$. The overall phase depends on the fixed insertion point $x$; it does not change the [energy eigenvalue](../../../../energy-eigenvalue-split.md). It cannot simply be dropped if the equality of complex [matrix elements](../../../../matrix-element.md) is to hold exactly.

The transformed state has [four-momentum](../../../../four-momentum.md) $q'=\Lambda q$. [Lorentz invariance](../../../../lorentz-invariance.md) of the [Minkowski inner product](../../../../minkowski-inner-product.md) gives

$$
p\cdot q=(\Lambda p)\cdot(\Lambda q)=m_\psi q'^0,
\qquad
\boxed{E^\Psi=\frac{p\cdot q}{m_\psi}=\frac{E_{\mathbf p}E_{\mathbf q}^{\chi}-\mathbf p\cdot\mathbf q}{m_\psi}.}
$$

There is no boost to a [rest frame](../../../../rest-frame.md) for a nonzero massless [four-momentum](../../../../four-momentum.md), so the rest-state statements require the positive-mass assumption.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
