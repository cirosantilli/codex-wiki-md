<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [smooth function](../../../../../smooth-function.md) $f$ and the [Levi-Civita connection](../../../../../levi-civita-connection.md) $\nabla$, the [Riemannian Hessian](../../../../../riemannian-hessian.md) is the covariant two-tensor

$$
\operatorname{Hess}_g f(X,Y)=(\nabla_Xdf)(Y)=X(Yf)-df(\nabla_XY).
$$

The connection rules show that this is linear over [smooth functions](../../../../../smooth-function.md) in both vector-field arguments, so it is a [tensor](../../../../../tensor.md). Torsion-freeness gives its symmetry:

$$
\operatorname{Hess}_g f(X,Y)-\operatorname{Hess}_g f(Y,X)
=[X,Y]f-df(\nabla_XY-\nabla_YX)=0.
$$

Its [metric trace](../../../../../metric-trace.md) defines the paper's [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md), $\Delta=\operatorname{div}_g\operatorname{grad}_g$; its [eigenvalues](../../../../../eigenvalue.md) on a [closed manifold](../../../../../closed-manifold.md) are nonpositive. We use $P=-\Delta$ when listing nonnegative [eigenvalues](../../../../../eigenvalue.md) or writing $e^{-tP}$.

At $p$, choose an [orthonormal basis](../../../../../orthonormal-basis.md) $e_1,\ldots,e_d$ of the [tangent space](../../../../../tangent-space.md) and unit-speed [geodesics](../../../../../geodesic.md) $\gamma_i(t)=\exp_p(te_i)$. Differentiating twice along a curve gives

$$
\frac{d^2}{dt^2}f(\gamma_i(t))
=\operatorname{Hess}_g f(\dot\gamma_i,\dot\gamma_i)+df(\nabla_{\dot\gamma_i}\dot\gamma_i).
$$

The covariant acceleration vanishes on a [geodesic](../../../../../geodesic.md). Taking the [trace](../../../../../matrix-trace.md) at $t=0$ proves the [geodesic trace formula for the Laplace-Beltrami operator](../../../../../geodesic-trace-formula-for-the-laplace-beltrami-operator.md):

$$
\boxed{\Delta f(p)=\sum_{i=1}^d(f\circ\gamma_i)''(0)
=\lim_{h\to0}\frac{\sum_{i=1}^d[f(\exp_p(he_i))+f(\exp_p(-he_i))-2f(p)]}{h^2}.}
$$

The last equality is Taylor's formula along the [geodesics](../../../../../geodesic.md), and expresses the [Laplacian](../../../../../laplacian.md) entirely through nearby function values.

For stabilization, let $X_1,X_2$ be the assumed isospectral nonisometric four-dimensional [tori](../../../../../torus.md), and let $k=n-4>0$. Take the same small [flat torus](../../../../../flat-torus.md) $F_\varepsilon=\mathbb R^k/\varepsilon\mathbb Z^k$ as an extra factor. On a [Riemannian product](../../../../../riemannian-product.md),

$$
P_{X_i\times F_\varepsilon}=P_{X_i}\otimes I+I\otimes P_{F_\varepsilon}.
$$

If $\phi_j$ and $\psi_\ell$ are [eigenfunctions](../../../../../eigenfunction.md) with [eigenvalues](../../../../../eigenvalue.md) $\lambda_j$ and $\mu_\ell$, then $\phi_j\psi_\ell$ has [eigenvalue](../../../../../eigenvalue.md) $\lambda_j+\mu_\ell$. Products of [orthonormal eigenbases](../../../../../orthonormal-eigenbasis.md) are complete in the product $L^2$ space, so this lists all [eigenvalues](../../../../../eigenvalue.md) with [multiplicities](../../../../../multiplicity-mathematics.md), including coincidences between different sums. Consequently the two products are isospectral.

One must also prove that multiplying by a common factor has not accidentally made the two [manifolds](../../../../../topological-manifold.md) [isometric](../../../../../isometry.md). Choose

$$
0<\varepsilon<\delta<\min\{\operatorname{inj}(X_1),\operatorname{inj}(X_2)\}.
$$

The injectivity radii are positive because the factors are [compact](../../../../../compact-space.md). A [closed](../../../../../closed-set.md) product [geodesic](../../../../../geodesic.md) of length less than $\delta$ projects to a [closed geodesic](../../../../../closed-geodesic.md) of length less than $\delta$ in $X_i$. Such a projected [geodesic](../../../../../geodesic.md) must be constant: otherwise its initial vector over one period would be a nonzero vector of norm below the [injectivity radius](../../../../../injectivity-radius.md) mapping back to its starting point under the [exponential map](../../../../../exponential-map-riemannian-geometry.md). Thus all sufficiently short [closed geodesics](../../../../../closed-geodesic.md) lie in the $F_\varepsilon$ directions. Conversely the $k$ coordinate circles, of length $\varepsilon$, pass through every point and span those directions.

It follows that the [smooth distribution](../../../../../distribution-differential-geometry.md) tangent to the small flat-torus factor is characterized intrinsically by the span of tangent vectors to [closed geodesics](../../../../../closed-geodesic.md) of length below $\delta$. A hypothetical product [isometry](../../../../../isometry.md) would preserve this [smooth distribution](../../../../../distribution-differential-geometry.md) and its [orthogonal complement](../../../../../orthogonal-complement.md). The latter has leaves $X_i\times\{q\}$; the [isometry](../../../../../isometry.md) and its inverse take whole leaves to whole leaves, thereby giving an [isometry](../../../../../isometry.md) $X_1\cong X_2$, a contradiction. This proves [isospectral stabilization by a small flat torus](../../../../../isospectral-stabilization-by-a-small-flat-torus.md):

$$
\boxed{X_1\times F_\varepsilon\text{ and }X_2\times F_\varepsilon\text{ are isospectral nonisometric }n\text{-tori for every }n>4.}
$$

This argument works even without assuming that the original four-dimensional [torus](../../../../../torus.md) metrics are flat.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
