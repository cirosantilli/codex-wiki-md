<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use coordinate indices $\mu,\nu$ and Lorentz-frame indices $A,B$, and take $\eta_{AB}=\operatorname{diag}(-1,1,1,1)$. Locally choose four independent one-forms $e^A=e^A{}_\mu dx^\mu$ satisfying

$$
\boxed{g_{\mu\nu}=\eta_{AB}e^A{}_\mu e^B{}_\nu.}
$$

One construction begins with a smooth timelike vector field in a sufficiently small neighborhood, normalizes it, and applies the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) to its spacelike orthogonal complement. The dual [orthonormal coframe in spacetime](../../../../../orthonormal-coframe-in-spacetime.md) gives the [vierbein](../../../../../orthonormal-coframe-in-spacetime.md); equivalently its matrix factorizes the metric as $g=e^T\eta e$. The inverse matrix gives the frame $e_A=e_A{}^\mu\partial_\mu$ with $e_A{}^\mu e^B{}_\mu=\delta_A^B$. This is a local construction: a global frame is not guaranteed by a metric, and a globally defined [spinor field](../../../../../spinor-field.md) requires a compatible [spin structure](../../../../../spin-structure.md).

The metric does not determine a unique [vierbein](../../../../../orthonormal-coframe-in-spacetime.md). A [local Lorentz transformation](../../../../../local-lorentz-transformation.md) changes the coframe components by

$$
\boxed{e'^A{}_\mu=\Lambda^A{}_B(x)e^B{}_\mu,\qquad
\Lambda^T\eta\Lambda=\eta,\qquad
e'_A{}^\mu=(\Lambda^{-1})^B{}_A e_B{}^\mu.}
$$

The coordinate index is unchanged in this frame transformation. Restrict to the proper orthochronous Lorentz group for its connected spin lift; orientation-reversing transformations require further structure and are not part of this local spin-group discussion.

Let constant [gamma matrices](../../../../../gamma-matrices.md) obey the [Clifford algebra](../../../../../clifford-algebra.md) $\{\gamma^A,\gamma^B\}=2\eta^{AB}$, and write $\gamma^{AB}=\tfrac12[\gamma^A,\gamma^B]$. A [spinor field](../../../../../spinor-field.md) transforms by the spin lift of the Lorentz transformation, not by its vector matrix:

$$
\boxed{\psi'(x)=S(\Lambda(x))\psi(x),\qquad
S^{-1}\gamma^A S=\Lambda^A{}_B\gamma^B.}
$$

For $\Lambda=1+\alpha+O(\alpha^2)$, with $\alpha_{AB}=-\alpha_{BA}$, the [Clifford algebra](../../../../../clifford-algebra.md) identity

$$
[\gamma^C,\gamma^{AB}]=2(\eta^{CA}\gamma^B-\eta^{CB}\gamma^A)
$$

shows explicitly that

$$
S=1+\frac14\alpha_{AB}\gamma^{AB}+O(\alpha^2).
$$

Indeed the commutator of $\gamma^C$ with this infinitesimal spin matrix is $\alpha^C{}_B\gamma^B$. A finite transformation connected to the identity is obtained by exponentiating these generators along a path. Its lift has two possible signs, so spinors are not ordinary Lorentz vectors: a $2\pi$ spatial rotation acts by $-1$, and $4\pi$ by $+1$. Consistent transition lifts define the [spin structure](../../../../../spin-structure.md); the metric alone does not select it.

For the metric connection, take the [Levi-Civita connection](../../../../../levi-civita-connection.md) and determine the [spin connection](../../../../../spin-connection.md) from the tetrad postulate

$$
\partial_\mu e^A{}_\nu+\omega_\mu{}^A{}_B e^B{}_\nu-\Gamma^\rho_{\mu\nu}e^A{}_\rho=0.
$$

It is equivalently determined by $de^A+\omega^A{}_B\wedge e^B=0$ and $\omega_{\mu AB}=-\omega_{\mu BA}$. Explicitly, in terms of the inverse frame,

$$
\omega_\mu{}^A{}_B=e^A{}_\nu\left(\partial_\mu e_B{}^\nu+\Gamma^\nu_{\mu\rho}e_B{}^\rho\right).
$$

Thus both the coordinate connection and the Lorentz [connection 1-form](../../../../../connection-1-form-split.md) are determined by the metric and chosen frame; no independent torsion has been supplied.

An ordinary derivative fails covariance because $\partial_\mu(S\psi)=S\partial_\mu\psi+(\partial_\mu S)\psi$. Seek $\nabla_\mu\psi=(\partial_\mu+\Omega_\mu)\psi$. Covariance requires

$$
\Omega'_\mu=S\Omega_\mu S^{-1}-(\partial_\mu S)S^{-1}.
$$

The coframe's connection obeys $\omega'=\Lambda\omega\Lambda^{-1}-d\Lambda\,\Lambda^{-1}$. Applying the spin representation of the same Lorentz algebra, whose infinitesimal generator was just determined, supplies

$$
\boxed{\nabla_\mu\psi=\partial_\mu\psi+\frac14\omega_{\mu AB}\gamma^{AB}\psi
=\partial_\mu\psi+\frac18\omega_{\mu AB}[\gamma^A,\gamma^B]\psi.}
$$

This proves the transformation law rather than choosing the coefficient arbitrarily. It is the [spinor covariant derivative](../../../../../spinor-covariant-derivative.md) induced by the [spin connection](../../../../../spin-connection.md). With curved matrices $\gamma^\nu(x)=e_A{}^\nu\gamma^A$, the same coefficient and tetrad postulate give

$$
\partial_\mu\gamma^\nu+\Gamma^\nu_{\mu\rho}\gamma^\rho+[\Omega_\mu,\gamma^\nu]=0,
$$

so differentiation is compatible with Clifford multiplication and $\{\gamma^\mu(x),\gamma^\nu(x)\}=2g^{\mu\nu}(x)$.

Finally, expand the commutator of these derivatives:

$$
[\partial_\mu+\Omega_\mu,\partial_\nu+\Omega_\nu]\psi
=(\partial_\mu\Omega_\nu-\partial_\nu\Omega_\mu+[\Omega_\mu,\Omega_\nu])\psi.
$$

The spin representation preserves the Lorentz algebra bracket. Consequently $d\Omega+\Omega\wedge\Omega=\tfrac14R_{AB}\gamma^{AB}$, where $R^A{}_B=d\omega^A{}_B+\omega^A{}_C\wedge\omega^C{}_B$. In components the [spinor curvature identity](../../../../../spinor-curvature-identity.md) is

$$
\boxed{[\nabla_\mu,\nabla_\nu]\psi=\frac14R_{\mu\nu AB}\gamma^{AB}\psi.}
$$

For the full second derivative, $\nabla_\mu(\nabla_\nu\psi)$ also includes $-\Gamma^\rho_{\mu\nu}\nabla_\rho\psi$, because its first derivative has a covector index. This term cancels on antisymmetrization for the [torsion-free connection](../../../../../torsion-free-connection.md). With unit-weight brackets, $X_{[\mu\nu]}=(X_{\mu\nu}-X_{\nu\mu})/2$, the requested expression is therefore

$$
\boxed{\nabla_{[\mu}\nabla_{\nu]}\psi
=\frac18R_{\mu\nu AB}\gamma^{AB}\psi
=\frac1{16}R_{\mu\nu AB}[\gamma^A,\gamma^B]\psi.}
$$

This convention distinguishes the antisymmetrized second derivative from the full commutator by its factor of two. In a noncoordinate orthonormal frame, an operator commutator must additionally subtract the derivative along the frame-vector commutator; using the full tensorial second derivative incorporates that correction.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
