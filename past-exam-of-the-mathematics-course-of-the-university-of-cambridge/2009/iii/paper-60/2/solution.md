<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [chirality matrix](../../../../../chirality-matrix.md) is covariantly constant under the metric-preserving [spin connection](../../../../../spin-connection.md) and anticommutes with every $\gamma^\mu$. Hence

$$
\not\nabla(\gamma_5\psi)=-\gamma_5\not\nabla\psi=m\gamma_5\psi,
\qquad
\boxed{(\not\nabla-m)\gamma_5\psi=0.}
$$

Thus multiplication by $\gamma_5$ reverses the sign of the mass parameter. At $m=0$ it maps solutions into solutions of the same [Dirac equation](../../../../../dirac-equation.md).

Use the [spinor curvature identity](../../../../../spinor-curvature-identity.md)

$$
[\nabla_\mu,\nabla_\nu]\psi=\frac14R_{\mu\nu ab}\gamma^{ab}\psi.
$$

Here the [rough Laplacian](../../../../../rough-laplacian.md) includes the affine connection on the index of the first derivative. Clifford expansion gives

$$
\not\nabla^2\psi
=\nabla^2\psi+\frac12\gamma^{\mu\nu}[\nabla_\mu,\nabla_\nu]\psi
=\nabla^2\psi+\frac18\gamma^{\mu\nu}R_{\mu\nu ab}\gamma^{ab}\psi.
$$

In the last contraction, the four-gamma part vanishes by the [first Bianchi identity](../../../../../first-bianchi-identity.md), the two-gamma parts vanish by symmetry of the [Ricci tensor](../../../../../ricci-tensor.md), and the scalar contractions give $-2R$. Therefore the [Lichnerowicz spinor-square formula](../../../../../lichnerowicz-spinor-square-formula.md) is

$$
\not\nabla^2=\nabla^2-\frac R4.
$$

Multiplying the first-order equation by $-\not\nabla+m$ now proves

$$
\boxed{\left(-\nabla^2+\frac R4+m^2\right)\psi=0.}
$$

The explicit curvature coefficient is fixed by the minimal spinor coupling; it is not an arbitrary scalar-field curvature coupling.

For the general metric-preserving connection, define $T^\rho{}_{\mu\nu}=\Gamma^\rho_{\mu\nu}-\Gamma^\rho_{\nu\mu}$ and let $R^T$ be its curvature. Distinguish the spin connection acting on the spinor from the full second derivative acting also on its derivative index. Their antisymmetric relation is

$$
\nabla^T_\mu\nabla^T_\nu\psi-\nabla^T_\nu\nabla^T_\mu\psi
=\frac14R^T_{\mu\nu ab}\gamma^{ab}\psi-T^\rho{}_{\mu\nu}\nabla^T_\rho\psi.
$$

Thus the [torsion correction to the Dirac square](../../../../../torsion-correction-to-the-dirac-square.md) gives the exact squared field equation

$$
\boxed{\left[-(\nabla^T)^2+\frac12\gamma^{\mu\nu}T^\rho{}_{\mu\nu}\nabla^T_\rho
-\frac18\gamma^{\mu\nu}R^T_{\mu\nu ab}\gamma^{ab}+m^2\right]\psi=0.}
$$

General torsion removes the curvature symmetries used in the preceding simplification. The curvature contraction may now contain nonscalar Clifford terms, in addition to the displayed first-order torsion term; simply replacing $R$ by a torsionful scalar in the torsion-free answer is not valid.

Equivalently, write the connection as Levi-Civita plus [contorsion tensor](../../../../../contorsion-tensor.md) $C_{\mu ab}$. Then $\not\nabla_T=\not\nabla_0+Q$, where $Q=\gamma^\mu C_{\mu ab}\gamma^{ab}/4$, and the square contains $\{\not\nabla_0,Q\}+Q^2$. This exhibits the extra couplings through derivatives of contorsion, first-order spinor derivatives and quadratic contorsion. Metric compatibility still preserves $\gamma_5$, so the mass-sign result remains valid. Spin therefore couples directly to curvature through its connection and the universal $R/4$ term, and to torsion through additional spin-dependent terms. The scalar reduction in the torsion-free square does not mean the full spinor transport is insensitive to the remaining Riemann curvature.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
