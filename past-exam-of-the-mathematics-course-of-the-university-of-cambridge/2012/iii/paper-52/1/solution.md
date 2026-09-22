<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use metric signature $+---$ and the [parity](../../../../../parity.md) matrix $P^\mu{}_{\nu}=\operatorname{diag}(1,-1,-1,-1)$. If a [Dirac field](../../../../../dirac-field.md) transforms as $\psi'(x)=\eta_P S_P\psi(x_P)$, the chain rule changes the spatial derivatives' signs. Covariance of its [Dirac equation](../../../../../dirac-equation.md) therefore requires

$$
S_P^{-1}\gamma^0S_P=\gamma^0,\qquad S_P^{-1}\gamma^iS_P=-\gamma^i.
$$

The [Clifford algebra](../../../../../clifford-algebra.md) gives precisely these identities for $S_P=\gamma^0$. In an irreducible Dirac representation any other solution differs by a scalar phase, because its ratio with $\gamma^0$ commutes with all [gamma matrices](../../../../../gamma-matrices.md). With $|\eta_P|=1$, the Dirac [mass](../../../../../mass.md) bilinear and [kinetic term](../../../../../kinetic-term.md) consequently obey

$$
\bar\psi'(x)\psi'(x)=\bar\psi(x_P)\psi(x_P),\qquad
\bar\psi'(x)i\gamma^\mu\partial_\mu\psi'(x)
=\bar\psi(x_P)i\gamma^\mu\partial_\mu\psi(x_P).
$$

**The factor $\gamma^0$ compensates the sign reversal of spatial derivatives.** A transformation containing only the argument change would not preserve the massive [Dirac equation](../../../../../dirac-equation.md). This establishes [parity](../../../../../parity.md) symmetry of the free or vector-coupled Dirac theory; it does not make a chiral [weak interaction](../../../../../weak-interaction.md) [parity](../../../../../parity.md) symmetric.

For [charge conjugation](../../../../../charge-conjugation.md), transpose the adjoint [Dirac equation](../../../../../dirac-equation.md) to obtain $(i\gamma^{\mu T}\partial_\mu+m)\bar\psi^T=0$. Multiplying by $C$ gives the original [Dirac equation](../../../../../dirac-equation.md) for $\psi^c=C\bar\psi^T$ if

$$
\boxed{C\gamma^{\mu T}C^{-1}=-\gamma^\mu,\qquad
C^{-1}\gamma^\mu C=-\gamma^{\mu T}.}
$$

One may choose $C$ unitary; in four dimensions a conventional choice in a standard Dirac or chiral basis is $C=i\gamma^2\gamma^0$, with $C^T=-C$. Its overall phase and $\eta_C$ do not affect the following bilinear transformation. Reordering the Grassmann [fermion](../../../../../fermion.md) fields gives, for a color matrix $X$ commuting with the [gamma matrices](../../../../../gamma-matrices.md),

$$
\overline{\psi^c}\gamma^\mu X\psi^c=-\bar\psi\gamma^\mu X^T\psi.
$$

Thus a vector color current changes sign and transposes its color generator under [charge conjugation](../../../../../charge-conjugation.md).

Write the Hermitian color connection as $\mathcal A_\mu=A_\mu^aT^a$. The interaction coming from $D_\mu=\partial_\mu+ig\mathcal A_\mu$ is $-g\bar\psi\gamma^\mu\mathcal A_\mu\psi$. Its charge-conjugation symmetry requires $\mathcal A_\mu^C=-\mathcal A_\mu^T$. [Parity](../../../../../parity.md) acts on the Lorentz index as on a vector connection, so combining the two gives

$$
\boxed{\mathcal A_\mu^{CP}(x)=-P_\mu{}^\nu\mathcal A_\nu^T(x_P).}
$$

In components, $\mathcal A_0\mapsto-\mathcal A_0^T(x_P)$ and $\mathcal A_i\mapsto+\mathcal A_i^T(x_P)$. The transpose is a color-space transpose, independent of the spinor matrix $C$. Intrinsic [fermion](../../../../../fermion.md) phases cancel between a field and its adjoint.

Define the matrix [gauge field strength](../../../../../gauge-field-strength.md) unambiguously by

$$
\mathcal F_{\mu\nu}=\partial_\mu\mathcal A_\nu-\partial_\nu\mathcal A_\mu+ig[\mathcal A_\mu,\mathcal A_\nu].
$$

The derivative terms transform with the expected [parity](../../../../../parity.md) factors and a minus transpose. For the commutator, the crucial identity is $[X^T,Y^T]=-[X,Y]^T$, so the nonlinear term has the same transformation as the derivative terms. This is the [CP transformation of non-Abelian field strength](../../../../../cp-transformation-of-non-abelian-field-strength.md):

$$
\boxed{\mathcal F_{\mu\nu}^{CP}(x)=-P_\mu{}^\alpha P_\nu{}^\beta\mathcal F_{\alpha\beta}^T(x_P).}
$$

For example, $\mathcal F_{0i}\mapsto+\mathcal F_{0i}^T(x_P)$ while $\mathcal F_{ij}\mapsto-\mathcal F_{ij}^T(x_P)$. With $\operatorname{tr}(T^aT^b)=\frac12\delta^{ab}$, the color sum in the theta operator is twice a [trace](../../../../../matrix-trace.md) of two field strengths. The two charge-conjugation minus signs cancel, and transposition reverses the [trace](../../../../../matrix-trace.md) factors without changing their [trace](../../../../../matrix-trace.md). The four [parity](../../../../../parity.md) matrices contracted with the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) contribute $\det P=-1$. Hence

$$
\boxed{\left[\epsilon^{\mu\nu\rho\sigma}F_{\mu\nu}^aF_{\rho\sigma}^a\right]^{CP}(x)
=-\epsilon^{\mu\nu\rho\sigma}F_{\mu\nu}^aF_{\rho\sigma}^a(x_P).}
$$

**The theta operator is [CP](../../../../../cp-symmetry.md) odd; a generic fixed nonzero coefficient violates [CP](../../../../../cp-symmetry.md).** Setting the coefficient to zero removes this term. Although the density is locally a total derivative, nontrivial gauge topology means that it need not be irrelevant to the quantum theory. If a properly normalized theta angle is identified periodically, invariance at special values equivalent to their negatives is a separate global question; it does not change the [CP](../../../../../cp-symmetry.md) odd transformation of the local operator.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
