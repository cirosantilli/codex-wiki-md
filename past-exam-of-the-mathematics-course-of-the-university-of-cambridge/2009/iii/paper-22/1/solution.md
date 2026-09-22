<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [musical isomorphisms](../../../../../musical-isomorphism.md) are the pointwise maps induced by the [Riemannian metric](../../../../../riemannian-metric.md):

$$
X^\flat(Y)=g(X,Y),\qquad g(\alpha^\sharp,Y)=\alpha(Y).
$$

In local coordinates they are $(X^\flat)_i=g_{ij}X^j$ and $(\alpha^\sharp)^i=g^{ij}\alpha_j$. The inverse metric makes these inverse bundle maps, hence inverse maps between smooth [vector fields](../../../../../vector-field.md) and smooth [differential one-forms](../../../../../one-form.md).

For a covariant two-tensor $\beta$, its [metric trace](../../../../../metric-trace.md) is $\operatorname{tr}_g\beta=g^{ij}\beta_{ij}=\sum_i\beta(e_i,e_i)$ in a [Riemannian orthonormal frame](../../../../../riemannian-orthonormal-frame.md). The contraction is independent of the chosen frame. There is a terminology distinction here: if $\beta$ is literally an alternating [differential two-form](../../../../../2-form.md), this trace is zero. The object needed below is the covariant two-tensor $D(X^\flat)$, generally not alternating. Interpreting that tensor as an alternating form would make the stated divergence construction impossible.

Let $D$ be the [Levi-Civita connection](../../../../../levi-civita-connection.md). The [Riemannian gradient](../../../../../riemannian-gradient.md), [divergence](../../../../../divergence.md) and positive [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) are

$$
\boxed{\operatorname{grad}_g f=(df)^\sharp,\qquad
\operatorname{div}_gX=\operatorname{tr}_gD(X^\flat),\qquad
\Delta_gf=-\operatorname{div}_g\operatorname{grad}_gf=-\operatorname{tr}_gDdf.}
$$

Thus $g(\operatorname{grad}_gf,Y)=Yf$, and in coordinates

$$
\Delta_gf=-\frac1{\sqrt{\det g}}\partial_i\left(\sqrt{\det g}\,g^{ij}\partial_j f\right).
$$

This choice makes the [Laplacian eigenvalues](../../../../../laplacian-eigenvalue.md) nonnegative on a closed [Riemannian manifold](../../../../../riemannian-manifold.md). The alternative convention $+\operatorname{div}\operatorname{grad}$ reverses all eigenvalue signs, but none of the comparisons below.

For the [Riemannian submersion](../../../../../riemannian-submersion.md), let $F=f\circ\pi$ and choose orthonormal horizontal lifts $E_i$ of a base frame and an orthonormal vertical frame $V_\alpha$. The horizontal part of $D_{E_i}E_i$ projects to the base [Levi-Civita connection](../../../../../levi-civita-connection.md); this follows directly from its [Koszul formula](../../../../../koszul-formula.md) applied to basic horizontal fields, because their inner products and projected brackets are pulled back from the base. Therefore the horizontal trace of the [Riemannian Hessian](../../../../../riemannian-hessian.md) of $F$ is the pulled-back base Hessian trace. Since $V_\alpha F=0$, its vertical terms are

$$
(DdF)(V_\alpha,V_\alpha)=-dF(D_{V_\alpha}V_\alpha).
$$

Writing $H=\sum_\alpha(D_{V_\alpha}V_\alpha)^{\mathrm{hor}}$ for the unnormalised fibre [mean curvature](../../../../../mean-curvature.md) vector gives

$$
\Delta_MF=(\Delta_Nf)\circ\pi+dF(H).
$$

The [totally geodesic submanifold](../../../../../totally-geodesic-submanifold.md) condition on the fibres makes $H=0$. Consequently [eigenfunction pullback by a Riemannian submersion](../../../../../eigenfunction-pullback-by-a-riemannian-submersion.md) gives

$$
\boxed{\pi^*:E_\lambda(N)\hookrightarrow E_\lambda(M),\qquad f\longmapsto f\circ\pi.}
$$

Here the [Riemannian submersion](../../../../../riemannian-submersion.md) is onto, so the map is injective. Its image is exactly the members of the upstairs [eigenspace](../../../../../eigenspace.md) constant on each whole fibre: such a function descends smoothly by local sections of the submersion, and the displayed identity forces the descended function to have the same [eigenvalue](../../../../../eigenvalue.md). In particular, whenever these [eigenspaces](../../../../../eigenspace.md) are finite dimensional, the downstairs multiplicity is no larger than the upstairs multiplicity. The upstairs [eigenspace](../../../../../eigenspace.md) may also contain functions varying along fibres.

A [flat torus](../../../../../flat-torus.md) is $\mathbb R^d/\Lambda$ with the metric induced by the [Euclidean metric](../../../../../euclidean-metric.md), where $\Lambda$ is a full-rank [Euclidean lattice](../../../../../euclidean-lattice.md). Its [dual lattice](../../../../../dual-lattice.md) is $\Lambda^*=\{w:\langle w,v\rangle\in\mathbb Z\text{ for all }v\in\Lambda\}$. The characters $e_w(x)=e^{2\pi i\langle w,x\rangle}$ descend to the quotient and form an orthogonal [Fourier basis](../../../../../fourier-basis.md) of $L^2$ on it. Direct differentiation gives the [spectrum of a flat torus](../../../../../spectrum-of-a-flat-torus.md):

$$
\boxed{\Delta e_w=4\pi^2|w|^2e_w,\qquad
\operatorname{Spec}(\mathbb R^d/\Lambda)=\{4\pi^2|w|^2:w\in\Lambda^*\},}
$$

with multiplicity equal to the number of [dual lattice](../../../../../dual-lattice.md) vectors of each length. In particular zero has multiplicity one.

Let the given four-dimensional [isospectral manifolds](../../../../../isospectral-manifolds.md) be $\mathbb R^4/\Lambda_1$ and $\mathbb R^4/\Lambda_2$. For $d=4+k$, take their products with the same $k$ circles of length $\varepsilon$, equivalently the lattices $\Lambda_i\oplus\varepsilon\mathbb Z^k$. The [dual lattices](../../../../../dual-lattice.md) are $\Lambda_i^*\oplus\varepsilon^{-1}\mathbb Z^k$, so their [Laplacian eigenvalues](../../../../../laplacian-eigenvalue.md) are

$$
4\pi^2\left(|w|^2+\varepsilon^{-2}|m|^2\right),\qquad
w\in\Lambda_i^*,\quad m\in\mathbb Z^k.
$$

The given equality of base [spectra](../../../../../spectrum-functional-analysis.md) with multiplicities makes these product [spectra](../../../../../spectrum-functional-analysis.md) identical.

Choose $\varepsilon$ smaller than the shortest nonzero vector length in either original [Euclidean lattice](../../../../../euclidean-lattice.md). By [short-vector cancellation for flat tori](../../../../../short-vector-cancellation-for-flat-tori.md), the shortest nonzero vectors in the product lattice are exactly $\pm\varepsilon e_j$ in its new factor. To spell out the nonisometry argument, any [isometry](../../../../../isometry.md) of the product [flat tori](../../../../../flat-torus.md) lifts to an [isometry](../../../../../isometry.md) of their universal Euclidean covers. This is affine, and its orthogonal linear part maps one product lattice onto the other. It must map the span of their shortest vectors, namely the new $k$-dimensional factor, onto itself; orthogonality then preserves the original four-dimensional factor and maps $\Lambda_1$ onto $\Lambda_2$. That would give an [isometry](../../../../../isometry.md) of the original [flat tori](../../../../../flat-torus.md), contrary to the assumption. **Isospectral nonisometric flat tori therefore exist in every dimension $d\geq4$.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
