<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the printed [gamma matrix](../../../../../../gamma-matrices.md) conventions throughout, in particular $\gamma^5=-i\gamma^0\gamma^1\gamma^2\gamma^3$. The transpose identity for $\gamma^0$ gives $C\gamma^0=-\gamma^0C$, and its [Hermitian conjugate](../../../../../../hermitian-conjugation.md) gives the corresponding identity for $C^\dagger$. Thus the [Dirac adjoint](../../../../../../dirac-adjoint.md) of the charge-conjugated field is

$$
\bar\psi^{\,C}=\eta_C^*\psi^T\gamma^0C^\dagger\gamma^0=-\eta_C^*\psi^TC^\dagger.
$$

Reordering the anticommuting components of the [fermion bilinear](../../../../../../fermion-bilinear.md) supplies a minus sign:

$$
\bar\psi^{\,C}\psi^C=-\psi^TC^\dagger C\bar\psi^T
=\bar\psi(C^\dagger C)^T\psi.
$$

Invariance for arbitrary fields therefore requires **$C^\dagger C=I$**, so the charge-conjugation matrix is a [unitary matrix](../../../../../../unitary-matrix.md). This is the required normalization constraint; it is not a bosonic reordering calculation.

For a spinor matrix $\Gamma$, the same calculation and the given $C^{-1}=C^T$ give

$$
(\bar\psi\Gamma\psi)^C=\bar\psi(C^{-1}\Gamma C)^T\psi
=\bar\psi C^{-1}\Gamma^TC\psi.
$$

With $V^\mu=\bar\psi\gamma^\mu\psi$ and $A^\mu=\bar\psi\gamma^\mu\gamma^5\psi$, the supplied transpose identities imply

$$
C^{-1}\gamma^{\mu T}C=-\gamma^\mu,\qquad
C^{-1}(\gamma^\mu\gamma^5)^TC
=-\gamma^5\gamma^\mu=\gamma^\mu\gamma^5.
$$

Consequently **the [vector current](../../../../../../vector-current.md) is C-odd and the [axial current](../../../../../../axial-current.md) is C-even**: $V^\mu\mapsto-V^\mu$ and $A^\mu\mapsto A^\mu$.

For [parity](../../../../../../parity.md), put $\Lambda=\operatorname{diag}(1,-1,-1,-1)$. The [gamma matrix](../../../../../../gamma-matrices.md) identities $\gamma^0\gamma^\mu\gamma^0=\Lambda^\mu{}_{\nu}\gamma^\nu$ and $\gamma^0\gamma^5\gamma^0=-\gamma^5$ give

$$
\boxed{V^\mu(x)\stackrel P\longmapsto\Lambda^\mu{}_{\nu}V^\nu(x_P),\qquad
A^\mu(x)\stackrel P\longmapsto-\Lambda^\mu{}_{\nu}A^\nu(x_P).}
$$

Thus $V^0$ is P-even and $\mathbf V$ P-odd, whereas $A^0$ is P-odd and $\mathbf A$ P-even. The [axial current](../../../../../../axial-current.md) transforms as a [pseudovector](../../../../../../pseudovector.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
