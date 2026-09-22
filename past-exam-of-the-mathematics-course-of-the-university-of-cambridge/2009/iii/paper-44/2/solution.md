<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The supplied matrices are the [chiral gamma-matrix representation](../../../../../chiral-gamma-matrix-representation.md). The [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) implies $\{\sigma^i,\sigma^j\}=2\delta^{ij}I_2$. Block multiplication gives $(\gamma^0)^2=I_4$, $\{\gamma^0,\gamma^i\}=0$, and $\{\gamma^i,\gamma^j\}=-2\delta^{ij}I_4$. Hence their [Clifford algebra](../../../../../clifford-algebra.md) relation is

$$
\boxed{\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}I_4.}
$$

Since partial derivatives commute, multiplying the [Dirac equation](../../../../../dirac-equation.md) by $i\gamma^\nu\partial_\nu+m$ gives

$$
0=(i\gamma^\nu\partial_\nu+m)(i\gamma^\mu\partial_\mu-m)\psi
=-(g^{\mu\nu}\partial_\mu\partial_\nu+m^2)\psi.
$$

Thus every component of the [Dirac spinor](../../../../../dirac-spinor.md) satisfies $\boxed{(\Box+m^2)\psi=0}$, the [Klein-Gordon equation](../../../../../klein-gordon-equation.md) with the same mass.

For a [Lorentz transformation](../../../../../lorentz-transformation.md) $x'=\Lambda x$, set $\psi'(x')=S(\Lambda)\psi(x)$. The derivative transforms as $\partial'_\mu=(\Lambda^{-1})^\nu{}_{\mu}\partial_\nu$. With the given spinor-matrix identity,

$$
S^{-1}(i\gamma^\mu\partial'_\mu-m)\psi'
=[i\Lambda^\mu{}_{\rho}\gamma^\rho(\Lambda^{-1})^\nu{}_{\mu}\partial_\nu-m]\psi
=(i\gamma^\nu\partial_\nu-m)\psi=0.
$$

This proves the [Lorentz covariance of the Dirac operator](../../../../../lorentz-covariance-of-the-dirac-operator.md) explicitly.

For [parity](../../../../../parity.md), let $x_P=(x^0,-\mathbf x)$ and $\psi_P(x)=\gamma^0\psi(x_P)$. Spatial differentiation brings a minus sign, which is canceled by $\gamma^i\gamma^0=-\gamma^0\gamma^i$. Therefore

$$
(i\gamma^\mu\partial_\mu-m)\psi_P(x)
=\gamma^0[(i\gamma^\mu\partial_\mu-m)\psi](x_P)=0.
$$

Since $\gamma^0$ is Hermitian and squares to one, the [Dirac adjoint](../../../../../dirac-adjoint.md) transforms as

$$
\boxed{\bar\psi_P(x)=\bar\psi(x_P)\gamma^0.}
$$

The [chirality matrix](../../../../../chirality-matrix.md) $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3$ anticommutes with $\gamma^0$. The [parity transformation of a Dirac bilinear](../../../../../parity-transformation-of-a-dirac-bilinear.md) consequently gives

$$
\boxed{\bar\psi_P\psi_P(x)=\bar\psi\psi(x_P),\qquad
\bar\psi_P\gamma^5\psi_P(x)=-\bar\psi\gamma^5\psi(x_P).}
$$

The first bilinear is a [Lorentz scalar](../../../../../lorentz-scalar.md) even under [parity](../../../../../parity.md), and the second is a [pseudoscalar](../../../../../pseudoscalar.md).

In this representation, $\gamma^5=\operatorname{diag}(-I_2,I_2)$. Its square is one, so the [chiral projectors](../../../../../chiral-projector.md) $P_\pm=(1\pm\gamma^5)/2$ are idempotent, mutually orthogonal and sum to the identity. They select $\psi_L=P_-\psi$ and $\psi_R=P_+\psi$, the two [Weyl spinors](../../../../../weyl-spinor.md). Because $\gamma^\mu P_\pm=P_\mp\gamma^\mu$, a solution of the [massless Dirac equation](../../../../../massless-dirac-equation.md) has each chiral component solving that equation separately. In two-component form,

$$
i(\partial_t-\boldsymbol\sigma\cdot\nabla)\psi_L=0,\qquad
i(\partial_t+\boldsymbol\sigma\cdot\nabla)\psi_R=0.
$$

The two [chirality](../../../../../chirality-physics.md) sectors are thus independent under massless propagation and proper [Lorentz transformations](../../../../../lorentz-transformation.md). A nonzero [Dirac mass term](../../../../../dirac-mass-term.md) couples them, while [parity](../../../../../parity.md) exchanges them. This explains why the projectors are particularly useful in the massless theory.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
