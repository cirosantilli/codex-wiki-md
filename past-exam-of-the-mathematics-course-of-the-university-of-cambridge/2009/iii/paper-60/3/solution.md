<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Work through terms quadratic in the fermions, with Grassmann-odd [Majorana spinors](../../../../../majorana-spinor.md) $\psi_\mu$ and $\epsilon$. At this order the [spin connection](../../../../../spin-connection.md) can be taken torsion-free: eliminating its gravitino-induced torsion changes the action only at four-fermion order. The Christoffel term needed to turn the printed $D_\nu\psi_\sigma$ into a full vector-spinor covariant derivative drops out after contraction with $\gamma^{\mu\nu\sigma}$, since the connection is symmetric in $\nu,\sigma$.

First establish the [Einstein tensor contraction of spin curvature](../../../../../einstein-tensor-contraction-of-spin-curvature.md). Expanding the Clifford product and using the [first Bianchi identity](../../../../../first-bianchi-identity.md), its five-gamma and antisymmetric three-gamma curvature contributions vanish, leaving

$$
\gamma^{\mu\nu\rho}R_{\nu\rho ab}\gamma^{ab}
=4R^\mu{}_\lambda\gamma^\lambda-2R\gamma^\mu.
$$

Since $[\nabla_\nu,\nabla_\rho]=R_{\nu\rho ab}\gamma^{ab}/4$, it follows that

$$
\boxed{\gamma^{\mu\nu\rho}\nabla_\nu\nabla_\rho\epsilon
=\frac12G^\mu{}_\lambda\gamma^\lambda\epsilon.}
$$

The factor $1/2$ arises from antisymmetrizing the two derivatives, not from a choice of Einstein-Hilbert normalization.

For the [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md), the metric variation is

$$
\delta g_{\mu\nu}=\frac\kappa2\bigl(\bar\psi_\mu\gamma_\nu\epsilon+\bar\psi_\nu\gamma_\mu\epsilon\bigr).
$$

Variation with respect to the covariant metric, including the determinant variation and discarding the usual boundary divergence, gives

$$
\delta S_{\rm EH}=-\frac1{2\kappa^2}\int |e|G^{\mu\nu}\delta g_{\mu\nu}\,d^4x
=-\frac1{2\kappa}\int |e|\bar\psi_\mu G^\mu{}_\lambda\gamma^\lambda\epsilon\,d^4x.
$$

No gravitational field equation has been assumed here.

For the [Rarita-Schwinger field](../../../../../rarita-schwinger-field.md) action, the determinant, gamma-matrix and connection variations each multiply a term already quadratic in $\psi$. Since $\delta e$ is bilinear in $\psi,\epsilon$, these contributions have four fermionic factors and are outside the requested order. Retain only the variations of the two explicit gravitino factors. The [four-dimensional Majorana bilinear interchange](../../../../../four-dimensional-majorana-bilinear-interchange.md) gives $\bar\chi\gamma^{\mu\nu\rho}\eta=\bar\eta\gamma^{\mu\nu\rho}\chi$ for odd spinors. After integration by parts, the first gravitino variation is

$$
\frac12\int |e|\overline{\delta\psi_\mu}\gamma^{\mu\nu\rho}\nabla_\nu\psi_\rho
=-\frac12\int |e|\bar\psi_\rho\gamma^{\mu\nu\rho}\nabla_\nu\delta\psi_\mu
=\frac12\int |e|\bar\psi_\mu\gamma^{\mu\nu\rho}\nabla_\nu\delta\psi_\rho,
$$

where the last step swaps $\mu,\rho$ and reverses the three-gamma sign. It is exactly equal to the variation of the second gravitino factor. Therefore

$$
\delta S_{\rm RS}=\int |e|\bar\psi_\mu\gamma^{\mu\nu\rho}\nabla_\nu\delta\psi_\rho
=\frac1\kappa\int |e|\bar\psi_\mu\gamma^{\mu\nu\rho}\nabla_\nu\nabla_\rho\epsilon
=\frac1{2\kappa}\int |e|\bar\psi_\mu G^\mu{}_\lambda\gamma^\lambda\epsilon.
$$

The curvature contribution cancels $\delta S_{\rm EH}$ pointwise. Thus

$$
\boxed{\delta(S_{\rm EH}+S_{\rm RS})=0}
$$

up to boundary terms and the omitted four-fermion-order variations. This directly proves the stated local [supersymmetry](../../../../../supersymmetry-split.md) invariance with its printed coefficients. At higher order, the torsion and quartic-fermion completion of [minimal four-dimensional supergravity](../../../../../minimal-four-dimensional-supergravity.md) is needed; it cannot be inferred by dropping the terms indefinitely.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
