<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) convention

$$
[\nabla_\mu,\nabla_\nu]\psi=\frac14R_{\mu\nu ab}\gamma^{ab}\psi,\qquad
\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu},
$$

with positive [scalar curvature](../../../../../scalar-curvature.md) for a round sphere. The connection preserves the gamma matrices. If $D=\gamma^\mu\nabla_\mu$, its square is

$$
D^2\psi=\nabla^2\psi+\frac12\gamma^{\mu\nu}[\nabla_\mu,\nabla_\nu]\psi
=\nabla^2\psi+\frac18\gamma^{\mu\nu}R_{\mu\nu ab}\gamma^{ab}\psi.
$$

Here $\nabla^2$ is the [rough Laplacian](../../../../../rough-laplacian.md), including the connection on the derivative index. In the product of two antisymmetric gamma pairs, the fully antisymmetric four-gamma term vanishes by the [first Bianchi identity](../../../../../first-bianchi-identity.md). The two-gamma contractions vanish because the [Ricci tensor](../../../../../ricci-tensor.md) is symmetric, while the scalar contractions give $-2R$. Thus the [Lichnerowicz spinor-square formula](../../../../../lichnerowicz-spinor-square-formula.md) is

$$
\boxed{D^2=\nabla^2-\frac R4.}
$$

Multiplying $(D+m)\psi=0$ by $-D+m$, with constant $m$, proves

$$
\boxed{-\nabla^2\psi+\frac R4\psi+m^2\psi=0.}
$$

In Riemannian signature $D$ in this positive-Clifford convention is formally [anti-self-adjoint](../../../../../skew-adjoint-generator.md); the more usual [self-adjoint](../../../../../self-adjoint-operator.md) Dirac operator $iD$ has square $-\nabla^2+R/4$. Stating this convention avoids an apparent sign conflict between the two forms of the formula.

Now let $D\psi=0$ on the compact Riemannian [spin manifold](../../../../../spin-manifold.md). Use the positive-definite spinor [inner product](../../../../../inner-product.md) and integrate the squared equation. [Integration by parts](../../../../../integration-by-parts.md) has no boundary contribution, giving

$$
0=\int_M\left(\langle\psi,-\nabla^2\psi\rangle+\frac R4|\psi|^2\right)dV
=\int_M\left(|\nabla\psi|^2+\frac R4|\psi|^2\right)dV.
$$

Both terms are nonnegative. Smoothness then forces $\nabla\psi=0$ pointwise. Consequently **every harmonic spinor is parallel**, and $R|\psi|^2=0$. A nonzero parallel spinor has constant positive norm on its connected component, so its [scalar curvature](../../../../../scalar-curvature.md) vanishes there. This is [compact harmonic-spinor rigidity under nonnegative scalar curvature](../../../../../compact-harmonic-spinor-rigidity-under-nonnegative-scalar-curvature.md).

The full Ricci conclusion follows from integrability, not merely from vanishing [scalar curvature](../../../../../scalar-curvature.md). Since a parallel spinor has zero curvature for its [spin connection](../../../../../spin-connection.md), contract its [Ricci identity](../../../../../curvature-commutator-on-a-covariant-tensor.md) with $\gamma^\nu$:

$$
0=\gamma^\nu[\nabla_\mu,\nabla_\nu]\psi
=\frac14R_{\mu\nu ab}\gamma^\nu\gamma^{ab}\psi
=-\frac12R_{\mu\nu}\gamma^\nu\psi.
$$

The three-gamma term vanishes by the [Bianchi identity](../../../../../bianchi-identity.md); the remaining contractions give the displayed Ricci term. For each fixed $\mu$, put $v_\nu=R_{\mu\nu}$. [Clifford multiplication](../../../../../clifford-multiplication.md) twice gives

$$
0=(v_\nu\gamma^\nu)^2\psi=|v|^2\psi.
$$

Positive definiteness and $\psi\ne0$ imply $v=0$. Thus the [Riemannian parallel-spinor Ricci-flatness](../../../../../riemannian-parallel-spinor-ricci-flatness.md) result is

$$
\boxed{R_{\mu\nu}=0.}
$$

On a connected manifold a nontrivial parallel solution is nowhere zero, so this holds everywhere. On a disconnected manifold it holds on every component supporting a nonzero spinor; the stated nowhere-vanishing hypothesis ensures all components are covered. The positive-definite [metric tensor](../../../../../metric-tensor.md) is essential to the last inference.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
