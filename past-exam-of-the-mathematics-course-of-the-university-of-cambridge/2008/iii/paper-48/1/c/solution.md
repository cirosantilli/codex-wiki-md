<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x'=\Lambda x$, choose the corresponding spin lift

$$
S(\Lambda)=\exp\!\left(\frac12\Omega_{\rho\sigma}M^{\rho\sigma}\right).
$$

The [spinor field](../../../../../../spinor-field.md) transforms as

$$
\boxed{\psi'(x')=S(\Lambda)\psi(x),\qquad
\psi'(x)=S(\Lambda)\psi(\Lambda^{-1}x).}
$$

The infinitesimal [Clifford algebra](../../../../../../clifford-algebra.md) identity from part (b) exponentiates to $S^{-1}\gamma^\mu S=\Lambda^\mu{}_{\nu}\gamma^\nu$, establishing [Lorentz covariance of the Dirac operator](../../../../../../lorentz-covariance-of-the-dirac-operator.md). At fixed coordinates the infinitesimal variation also includes the orbital term $-\Omega^\mu{}_{\nu}x^\nu\partial_\mu\psi$.

A spatial rotation generator $M^{ij}$ is anti-Hermitian, but a [Lorentz boost](../../../../../../lorentz-boost.md) generator is Hermitian. For example,

$$
M^{01}=\frac12\gamma^0\gamma^1
=\frac12\begin{pmatrix}-\sigma^1&0\\0&\sigma^1\end{pmatrix}.
$$

Its eigenvalues are $\pm\tfrac12$. A nonzero rapidity $\zeta$ gives boost eigenvalues $e^{\pm\zeta/2}$, which are not all on the unit circle. This proves that the finite-dimensional component [Spinor representation of the Lorentz group](../../../../../../spinor-representation-of-the-lorentz-group.md) cannot be unitary for a positive-definite component inner product, even after a change of basis. It does not contradict a unitary action on the physical space of quantum states.

Consequently $\psi'^\dagger(x')\psi'(x')=\psi^\dagger S^\dagger S\psi$ need not equal $\psi^\dagger\psi$: it is the time component of the [Dirac current](../../../../../../dirac-current.md), not a [Lorentz scalar](../../../../../../lorentz-scalar.md). The appropriate invariant form is indefinite. From $(\gamma^\mu)^\dagger=\gamma^0\gamma^\mu\gamma^0$ one obtains

$$
(M^{\rho\sigma})^\dagger\gamma^0+\gamma^0M^{\rho\sigma}=0,
\qquad S^\dagger\gamma^0S=\gamma^0.
$$

This [Dirac spinor pseudo-unitarity](../../../../../../dirac-spinor-pseudo-unitarity.md) gives $\bar\psi'(x')=\bar\psi(x)S^{-1}$ and hence the [Dirac scalar bilinear](../../../../../../dirac-scalar-bilinear.md)

$$
\boxed{\bar\psi'(x')\psi'(x')=\bar\psi(x)\psi(x).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
