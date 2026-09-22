<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the nonnegative sign convention $\Delta=-\operatorname{div}\operatorname{grad}$ for the [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md); the ambient [Laplacian](../../../../../laplacian.md) has the same sign convention. Changing both signs changes the signs of the [eigenvalues](../../../../../eigenvalue.md) below. Let $e_1,\ldots,e_n$ be an [orthonormal basis](../../../../../orthonormal-basis.md) of $T_pM$, and let $\gamma_i$ be the unit-speed [geodesic](../../../../../geodesic.md) with $\gamma_i(0)=p$ and $\dot\gamma_i(0)=e_i$. The [geodesic Hessian formula](../../../../../geodesic-hessian-formula.md) gives

$$
\boxed{\Delta f(p)=-\sum_{i=1}^n\left.\frac{d^2}{dt^2}f(\gamma_i(t))\right|_{t=0}.}
$$

Indeed, the second derivative along a [geodesic](../../../../../geodesic.md) is $\operatorname{Hess}f(e_i,e_i)$, because its covariant acceleration is zero. Taking the [trace](../../../../../matrix-trace.md) of the [Hessian matrix](../../../../../hessian-matrix.md) in this [orthonormal basis](../../../../../orthonormal-basis.md) gives the displayed [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md).

For the [sphere](../../../../../sphere.md), put $x=r\omega$, where $\omega\in S^d$, and write $F(r,\omega)$ for a smooth ambient function. The [Euclidean metric](../../../../../euclidean-metric.md) becomes $dr^2+r^2g_{S^d}$ and its [volume form](../../../../../volume-form.md) is $r^d\,dr\,d\omega$. The coordinate formula for the [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) therefore gives the [polar-coordinate Laplacian identity](../../../../../polar-coordinate-laplacian-identity.md)

$$
\widetilde\Delta F=-\partial_r^2F-\frac d r\partial_rF+\frac1{r^2}\Delta_{S^d}F.
$$

For $f(\omega)=F(1,\omega)$, restriction to $r=1$ yields

$$
\boxed{\Delta_{S^d}f=\left(\widetilde\Delta F+\partial_r^2F+d\partial_rF\right)\big|_{r=1}.}
$$

This relation also has a direct [geodesic](../../../../../geodesic.md) proof. At a point $p\in S^d$, complete an [orthonormal basis](../../../../../orthonormal-basis.md) of the tangent space by the radial vector $p$. Each great-circle [geodesic](../../../../../geodesic.md) $\gamma_i(t)=p\cos t+e_i\sin t$ satisfies $\ddot\gamma_i(0)=-p$. The chain rule gives $(F\circ\gamma_i)''(0)=D^2F(e_i,e_i)-\partial_rF$. Summing and comparing with the ambient [trace](../../../../../matrix-trace.md) gives precisely the radial correction above.

Let $\mathcal P_\ell$ be the space of [homogeneous polynomials](../../../../../homogeneous-polynomial.md) of degree $\ell$ on $\mathbb R^{d+1}$, and let $\mathcal H_\ell$ be its subspace of [harmonic polynomials](../../../../../harmonic-polynomial.md). For $H\in\mathcal H_\ell$, homogeneity gives $H(r\omega)=r^\ell H(\omega)$. Substituting in the [polar-coordinate Laplacian identity](../../../../../polar-coordinate-laplacian-identity.md) proves that its restriction $h$ is a [spherical harmonic](../../../../../spherical-harmonic.md) with

$$
\Delta_{S^d}h=\ell(\ell+d-1)h.
$$

Restriction is injective on $\mathcal H_\ell$: if $h=0$, homogeneity makes $H$ zero away from the origin, hence everywhere.

To count and exhaust these [eigenfunctions](../../../../../eigenfunction.md), use the [harmonic decomposition of homogeneous polynomials](../../../../../harmonic-decomposition-of-homogeneous-polynomials.md)

$$
\mathcal P_\ell=\mathcal H_\ell\oplus r^2\mathcal P_{\ell-2},\qquad \mathcal P_j=0\text{ for }j<0.
$$

Here is an algebraic proof rather than an assumption about the [spectrum](../../../../../spectrum-functional-analysis.md). On [polynomials](../../../../../polynomial-split.md) put the [Fischer inner product](../../../../../fischer-inner-product.md) $\langle x^\alpha,x^\beta\rangle_F=\alpha!\,\delta_{\alpha\beta}$. Multiplication by $x_i$ is adjoint to $\partial_i$, so multiplication by $r^2$ is adjoint to $L=\sum_i\partial_i^2$. In finite-dimensional [inner product spaces](../../../../../inner-product-space.md), the orthogonal complement of the image of multiplication by $r^2$ is $\ker L=\mathcal H_\ell$. This proves the decomposition. Multiplication by $r^2$ is injective, so

$$
\dim\mathcal H_\ell=\binom{\ell+d}{d}-\binom{\ell+d-2}{d},
$$

where the second term is zero for $\ell<2$.

Iterating the [harmonic decomposition of homogeneous polynomials](../../../../../harmonic-decomposition-of-homogeneous-polynomials.md) and restricting to $r=1$ expresses every polynomial restriction as a finite sum of [spherical harmonics](../../../../../spherical-harmonic.md). Polynomial restrictions contain constants and separate points of the [sphere](../../../../../sphere.md), so the [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) makes them uniformly dense in the continuous functions, and hence dense in $L^2(S^d)$. The [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) is [self-adjoint](../../../../../self-adjoint-operator.md), and [eigenfunctions](../../../../../eigenfunction.md) with different [eigenvalues](../../../../../eigenvalue.md) are [orthogonal](../../../../../orthogonal-vectors.md). If a smooth [eigenfunction](../../../../../eigenfunction.md) had an [eigenvalue](../../../../../eigenvalue.md) not in the list, it would be orthogonal to a dense subspace and would vanish. If it had a listed [eigenvalue](../../../../../eigenvalue.md), subtracting its orthogonal projection onto the corresponding finite-dimensional $\mathcal H_\ell|_{S^d}$ gives the same contradiction. Thus, for $d\geq1$, the [spectrum of the Laplacian on a sphere](../../../../../spectrum-of-the-laplacian-on-a-sphere.md) is

$$
\boxed{\lambda_\ell=\ell(\ell+d-1),\quad
m_\ell=\binom{\ell+d}{d}-\binom{\ell+d-2}{d},\quad \ell=0,1,2,\ldots.}
$$

In particular, the zero [eigenvalue](../../../../../eigenvalue.md) has multiplicity one; on $S^1$ each positive [eigenvalue](../../../../../eigenvalue.md) $\ell^2$ has multiplicity two; on $S^2$ the multiplicity is $2\ell+1$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 117](../../paper-117-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
