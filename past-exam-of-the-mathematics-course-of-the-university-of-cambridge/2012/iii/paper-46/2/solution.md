<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Continue with metric signature $+---$. The Pauli matrices obey $\{\sigma^i,\sigma^j\}=2\delta^{ij}I_2$. Block multiplication in the [chiral gamma-matrix representation](../../../../../chiral-gamma-matrix-representation.md) gives

$$
(\gamma^0)^2=I_4,\qquad
\gamma^0\gamma^i=\begin{pmatrix}-\sigma^i&0\\0&\sigma^i\end{pmatrix},\qquad
\gamma^i\gamma^0=-\gamma^0\gamma^i,
$$

and

$$
\gamma^i\gamma^j=-\begin{pmatrix}\sigma^i\sigma^j&0\\0&\sigma^i\sigma^j\end{pmatrix}.
$$

Hence **$\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}I_4$**, the required [Clifford algebra](../../../../../clifford-algebra.md). Multiplying the [Dirac equation](../../../../../dirac-equation.md) by $i\gamma^\nu\partial_\nu+m$ yields

$$
(i\gamma^\nu\partial_\nu+m)(i\gamma^\mu\partial_\mu-m)\psi
=-(\Box+m^2)\psi=0.
$$

The antisymmetric part of $\gamma^\nu\gamma^\mu$ drops out because partial derivatives commute. Therefore every component of the [Dirac spinor](../../../../../dirac-spinor.md) satisfies the [Klein-Gordon equation](../../../../../klein-gordon-equation.md). The converse is not true: four arbitrary scalar solutions need not obey the first-order [Dirac equation](../../../../../dirac-equation.md).

The [Lorentz group](../../../../../lorentz-group.md) consists of real invertible matrices $\Lambda$ preserving the [Minkowski metric](../../../../../minkowski-metric.md): $\Lambda^Tg\Lambda=g$. Writing $\Lambda=I+\omega+O(\omega^2)$ gives $\omega_{\mu\nu}=-\omega_{\nu\mu}$, so **there are six continuous parameters: three spatial rotation angles and three boost rapidities**. The [Proper orthochronous Lorentz group](../../../../../proper-orthochronous-lorentz-group.md) is the connected component with determinant $+1$ that preserves time orientation. [Parity](../../../../../parity.md) and [time reversal](../../../../../t-symmetry.md) are additional discrete operations and are not encoded by the six real parameters in an exponential near the identity.

For the real-generator convention used here, vector generators can be written

$$
(M_{\rm vec}^{\rho\sigma})^\mu{}_{\nu}
=g^{\rho\mu}\delta^\sigma{}_{\nu}-g^{\sigma\mu}\delta^\rho{}_{\nu}.
$$

Take $\Omega_{\rho\sigma}=-\Omega_{\sigma\rho}$ and use the same parameters in the spinor representation. The [Lorentz-spinor generators from a Clifford algebra](../../../../../lorentz-spinor-generators-from-a-clifford-algebra.md) are

$$
\boxed{M_{\rm sp}^{\rho\sigma}=\frac14[\gamma^\rho,\gamma^\sigma],\qquad
S(\Lambda)=\exp\left(\frac12\Omega_{\rho\sigma}M_{\rm sp}^{\rho\sigma}\right).}
$$

To verify the [Lorentz algebra](../../../../../lorentz-algebra.md), first commute a generator with one [gamma matrix](../../../../../gamma-matrices.md):

$$
[M_{\rm sp}^{\rho\sigma},\gamma^\tau]
=g^{\sigma\tau}\gamma^\rho-g^{\rho\tau}\gamma^\sigma.
$$

For example, this follows by moving $\gamma^\tau$ through each product using the Clifford [anticommutator](../../../../../anticommutator.md). Applying the commutator derivation rule to $\frac14[\gamma^\tau,\gamma^\nu]$ then gives

$$
[M_{\rm sp}^{\rho\sigma},M_{\rm sp}^{\tau\nu}]
=g^{\sigma\tau}M_{\rm sp}^{\rho\nu}-g^{\rho\tau}M_{\rm sp}^{\sigma\nu}
+g^{\rho\nu}M_{\rm sp}^{\sigma\tau}-g^{\sigma\nu}M_{\rm sp}^{\rho\tau}.
$$

No extra factor of $i$ belongs in these generators with this commutator convention. Hermitian-generator conventions shift the factors of $i$ into the brackets and the exponential instead.

The same gamma commutator proves

$$
S^{-1}\gamma^\mu S=\Lambda^\mu{}_{\nu}\gamma^\nu.
$$

Indeed, to first order $S^{-1}\gamma^\mu S=\gamma^\mu+\frac12\Omega_{\rho\sigma}[\gamma^\mu,M_{\rm sp}^{\rho\sigma}]$, exactly the infinitesimal vector [action](../../../../../action.md) defined above. Exponentiating proves the finite relation. The spinor field transforms as **$\psi'(x')=S(\Lambda)\psi(x)$ with $x'=\Lambda x$**; combining this relation with $\partial'_\mu=(\Lambda^{-1})^\nu{}_{\mu}\partial_\nu$ preserves the [Dirac equation](../../../../../dirac-equation.md). A $2\pi$ rotation gives $S=-I_4$, so the spinor matrices give the double-cover [spin](../../../../../spin.md) representation, rather than a single-valued ordinary representation of the [Lorentz group](../../../../../lorentz-group.md) itself.

For a boost in direction $i$, $M_{\rm sp}^{0i}=\frac12\gamma^0\gamma^i$ is Hermitian, with eigenvalues $\pm\frac12$. A real [rapidity](../../../../../rapidity.md) $\eta$ therefore produces eigenvalues $e^{\pm\eta/2}$ in $S$, whose moduli are not one. **The finite-component spinor representation is not unitary for boosts**, although the rotation matrices are unitary. The [Lorentz group](../../../../../lorentz-group.md) is noncompact; this does not forbid the unitary infinite-dimensional [action](../../../../../action.md) on the physical Hilbert space of states.

Nevertheless, since $(\gamma^\mu)^\dagger=\gamma^0\gamma^\mu\gamma^0$,

$$
(M_{\rm sp}^{\rho\sigma})^\dagger\gamma^0+\gamma^0M_{\rm sp}^{\rho\sigma}=0,
\qquad S^\dagger\gamma^0S=\gamma^0.
$$

This [Dirac spinor pseudo-unitarity](../../../../../dirac-spinor-pseudo-unitarity.md) implies $\bar\psi'(x')=\bar\psi(x)S^{-1}$, and consequently

$$
\boxed{\bar\psi'(x')\psi'(x')=\bar\psi(x)\psi(x).}
$$

The [Dirac adjoint](../../../../../dirac-adjoint.md) is precisely the adjoint needed to form this [Lorentz scalar](../../../../../lorentz-scalar.md); ordinary $\psi^\dagger\psi$ alone is not a scalar.

Let $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3=\operatorname{diag}(-I_2,I_2)$. It anticommutes with every [gamma matrix](../../../../../gamma-matrices.md) and commutes with every $M_{\rm sp}^{\rho\sigma}$, so $S^{-1}\gamma^5S=\gamma^5$. Thus the [axial current](../../../../../axial-current.md) transforms as a [four-vector](../../../../../four-vector.md) under proper [Lorentz transformations](../../../../../lorentz-transformation.md):

$$
j_5'{}^\mu(x')=\Lambda^\mu{}_{\nu}j_5^\nu(x).
$$

Under [parity](../../../../../parity.md) it is an [axial vector](../../../../../pseudovector.md), acquiring the additional [pseudovector](../../../../../pseudovector.md) sign. Contracting two [axial currents](../../../../../axial-current.md) cancels that sign and uses the invariant metric. Therefore **$j_{5\mu}j_5^\mu$ is compatible with [Lorentz invariance](../../../../../lorentz-invariance.md)**, including [parity](../../../../../parity.md) invariance of this contraction. [Lorentz invariance](../../../../../lorentz-invariance.md) of the interaction does not require the [axial current](../../../../../axial-current.md) to be conserved.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
