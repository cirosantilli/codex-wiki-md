<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md) $\Delta=-\operatorname{div}\operatorname{grad}$. A [Riemannian submersion](../../../../../riemannian-submersion.md) is a surjective smooth [submersion](../../../../../submersion.md) $\pi:(M,g)\to(N,h)$ for which, at every $p$, the restriction of $d\pi_p$ to $H_p=(\ker d\pi_p)^\perp$ is a [linear isometry](../../../../../linear-isometry-of-hilbert-spaces.md) onto $T_{\pi(p)}N$. The spaces $V_p=\ker d\pi_p$ and $H_p$ are its vertical and horizontal spaces. Its [fibres](../../../../../fiber-of-a-function.md) are [totally geodesic submanifolds](../../../../../totally-geodesic-submanifold.md) precisely when $\nabla_UV$ is vertical for vertical [vector fields](../../../../../vector-field.md) $U,V$: their [second fundamental form](../../../../../second-fundamental-form-split.md) vanishes. Equivalently, a [geodesic](../../../../../geodesic.md) initially tangent to a fibre remains in that fibre while defined.

For a smooth $f:N\to\mathbb R$, its [basic function](../../../../../basic-function.md) $F=f\circ\pi$ is constant along each fibre. The [Riemannian gradient](../../../../../riemannian-gradient.md) of $F$ is the [horizontal lift of a vector field through a submersion](../../../../../horizontal-lift-of-a-vector-field-through-a-submersion.md) of $\operatorname{grad}_Nf$, since

$$
g(\operatorname{grad}_MF,X)=dF(X)=df(d\pi X)=h(\operatorname{grad}_Nf,d\pi X)
$$

for horizontal $X$, and $dF(U)=0$ for vertical $U$. In particular no derivative of $f$ in a vertical direction occurs.

Here is the needed connection fact, which also follows directly from the [Koszul formula](../../../../../koszul-formula.md): for horizontal lifts $X,Y$ of [vector fields](../../../../../vector-field.md) $\bar X,\bar Y$ on $N$, the horizontal component of $\nabla_XY$ projects to $\nabla^N_{\bar X}\bar Y$. To see this, pair the [Koszul formula](../../../../../koszul-formula.md) with a third horizontal lift $Z$. The horizontal [inner products](../../../../../inner-product.md) are pulled back from $N$, and the horizontal components of their [Lie brackets of vector fields](../../../../../lie-bracket-of-vector-fields.md) project to the brackets on $N$. Thus all six terms are the pullbacks of the corresponding terms on $N$.

Choose an adapted [Riemannian orthonormal frame](../../../../../riemannian-orthonormal-frame.md) $X_1,\ldots,X_n,U_1,\ldots,U_r$, with the $X_a$ horizontal lifts. Using $\operatorname{Hess}F(A,A)=A(AF)-(\nabla_AA)F$, the connection fact gives

$$
\operatorname{Hess}_MF(X_a,X_a)=(\operatorname{Hess}_Nf)(\bar X_a,\bar X_a)\circ\pi.
$$

For a vertical $U_b$, both $U_bF=0$ and $(\nabla_{U_b}U_b)F=0$, the latter because the fibres are [totally geodesic submanifolds](../../../../../totally-geodesic-submanifold.md). Taking the negative [metric trace](../../../../../metric-trace.md) of the [Riemannian Hessian](../../../../../riemannian-hessian.md) therefore proves the [basic-function Laplacian identity](../../../../../basic-function-laplacian-identity.md)

$$
\boxed{\Delta_M(f\circ\pi)=(\Delta_N f)\circ\pi.}
$$

This identity is local and does not require [compactness](../../../../../compact-space.md). Vanishing [mean curvature](../../../../../mean-curvature.md) of the [fibres](../../../../../fiber-of-a-function.md) would already suffice; total geodesicity makes each vertical summand vanish separately.

For the discrete [eigenspace](../../../../../eigenspace.md) assertion, assume the two [Riemannian manifolds](../../../../../riemannian-manifold.md) are [closed manifolds](../../../../../closed-manifold.md). Without a discrete spectral realization, an unrestricted noncompact version need not have an [eigenbasis](../../../../../eigenbasis.md). The projections of the [Riemannian product](../../../../../riemannian-product.md) $M\times N$ are [Riemannian submersions](../../../../../riemannian-submersion.md) with [totally geodesic submanifolds](../../../../../totally-geodesic-submanifold.md) as fibres. Its [Levi-Civita connection](../../../../../levi-civita-connection.md) splits into the two factor connections. Consequently its [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md) is

$$
\Delta_{M\times N}=\Delta_M\otimes I+I\otimes\Delta_N,
\qquad
\Delta_{M\times N}(u(x)v(y))=(\Delta_Mu)(x)v(y)+u(x)(\Delta_Nv)(y).
$$

The cross term in the [product rule for the positive Laplace-Beltrami operator](../../../../../product-rule-for-the-positive-laplace-beltrami-operator.md) is zero because the two factor [Riemannian gradients](../../../../../riemannian-gradient.md) are [orthogonal](../../../../../orthogonal-vectors.md).

We use the standard compact elliptic [compact elliptic spectral theorem](../../../../../compact-elliptic-spectral-theorem.md): the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md) on a [closed manifold](../../../../../closed-manifold.md) is [self-adjoint](../../../../../self-adjoint-operator.md), has [compact resolvent](../../../../../compact-resolvent.md), and has a complete [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) of smooth [eigenfunctions](../../../../../eigenfunction.md), with finite-dimensional [eigenspaces](../../../../../eigenspace.md) and [eigenvalues](../../../../../eigenvalue.md) tending to infinity. Let $\Delta_Mu_i=\mu_i u_i$ and $\Delta_Nv_j=\nu_jv_j$. [Fubini's theorem](../../../../../fubini-s-theorem.md) and completeness on each factor show that $u_i(x)v_j(y)$ form a complete [orthonormal basis](../../../../../orthonormal-basis.md) of $L^2(M\times N)$. For example, a function orthogonal to all these products has, for each $i$, zero $u_i$-coefficient as an $L^2(N)$ function, hence is zero.

The displayed operator identity makes $u_i v_j$ an [eigenfunction](../../../../../eigenfunction.md) with [eigenvalue](../../../../../eigenvalue.md) $\mu_i+\nu_j$. Conversely, if $\Delta w=\lambda w$, self-adjointness of the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md) gives

$$
(\mu_i+\nu_j-\lambda)\langle w,u_i v_j\rangle=0.
$$

All other coefficients vanish. Only finitely many pairs can have $\mu_i+\nu_j=\lambda$, since both [spectra](../../../../../spectrum-functional-analysis.md) are nonnegative and have finitely many [eigenvalues](../../../../../eigenvalue.md) below any fixed bound. Thus the [product Laplacian eigenspace decomposition](../../../../../product-laplacian-eigenspace-decomposition.md) is

$$
\boxed{E_\lambda(M\times N)=\bigoplus_{\mu+\nu=\lambda} E_\mu(M)\otimes E_\nu(N).}
$$

The [tensor product](../../../../../tensor-product.md) summands are mutually [orthogonal](../../../../../orthogonal-vectors.md); their elements are actual smooth [eigenfunctions](../../../../../eigenfunction.md), so this is an equality of [eigenspaces](../../../../../eigenspace.md), not just a formal expansion.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
