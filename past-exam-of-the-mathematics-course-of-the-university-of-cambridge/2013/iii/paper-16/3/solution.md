<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $M$ be a [closed manifold](../../../../../closed-manifold.md) with a [Riemannian metric](../../../../../riemannian-metric.md) and use $\Delta=-\operatorname{div}\operatorname{grad}$, the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md). This is the setting in which the final discrete [eigenfunction expansion](../../../../../eigenfunction-expansion.md) applies without additional boundary or noncompact spectral hypotheses. A [Riemannian heat kernel](../../../../../riemannian-heat-kernel.md) is a smooth $H(t,x,y)$ for $t>0$ such that

$$
(\partial_t+\Delta_x)H=0,\qquad
u(t,x)=\int_M H(t,x,y)f(y)\,dV_y\longrightarrow f(x)\quad(t\downarrow0)
$$

for every smooth initial function $f$. Here $\nu$ solves the [heat equation](../../../../../heat-equation.md). The limit is the statement that the initial kernel is the [Dirac delta distribution](../../../../../dirac-delta-function.md) on the diagonal. In the closed setting this uniquely determines the [heat kernel](../../../../../heat-kernel.md); it is symmetric, preserves constants, is nonnegative, and satisfies the [semigroup property](../../../../../semigroup-property.md).

A [heat parametrix](../../../../../heat-parametrix.md) $P(t,x,y)$ is an approximate version with the same delta initial limit and with error

$$
R=(\partial_t+\Delta_x)P
$$

regular enough at $t=0$ to correct by a convergent integral series. One may construct it by the local Gaussian ansatz

$$
P(t,x,y)=\chi(x,y)(4\pi t)^{-m/2}e^{-d(x,y)^2/(4t)}\sum_{j=0}^{q}t^j u_j(x,y),
$$

where $\chi=1$ near the diagonal and is supported in a [convex normal neighborhood](../../../../../convex-normal-neighbourhood.md), and the smooth coefficients solve the usual radial transport equations. The leading coefficient accounts for the [Riemannian volume form](../../../../../riemannian-volume-form.md). Taking $q$ sufficiently large makes the residual extend continuously, with any prescribed finite number of derivatives, to $t=0$. Alternatively a smooth asymptotic summation of all transport coefficients gives a residual vanishing to every order. These local construction, extension and differentiability facts are used here as subsidiary results, as permitted.

For the correction proof take a [heat parametrix](../../../../../heat-parametrix.md) whose residual is smooth up to $t=0$ on a short interval $[0,T]$. We also use its uniform integral bound $\sup_{0<t\le T,x}\int_M|P(t,x,y)|\,dV_y<\infty$, its approximate-identity limit, and the following standard differentiability property: convolution with a smooth time-dependent kernel gives a smooth kernel for $t>0$, and differentiating it yields the identity below. These properties follow from the Gaussian estimates and the delta initial limit; no conclusion about the final exact [heat kernel](../../../../../heat-kernel.md) is assumed.

Define the [Volterra convolution of kernels](../../../../../volterra-convolution-of-kernels.md) by

$$
(A*B)(t,x,y)=\int_0^t\int_M A(t-s,x,z)B(s,z,y)\,dV_z\,ds.
$$

It is associative wherever these integrals converge. The delta term at the upper endpoint gives

$$
(\partial_t+\Delta_x)(P*B)=B+R*B.
$$

Seek $H=P+P*Q$. Then its error vanishes exactly when $Q+R+R*Q=0$. The solution is the [Volterra parametrix correction](../../../../../volterra-parametrix-correction.md)

$$
Q=\sum_{k=1}^{\infty}(-1)^kR^{*k},\qquad H=P+P*Q.
$$

The signs matter: the first correction is $-P*R$.

To prove convergence, let $|R|\le C$ and $V=\operatorname{vol}(M)$. The time variables in $R^{*k}$ range over a simplex of volume $t^{k-1}/(k-1)!$, so

$$
|R^{*k}(t,x,y)|\le C^k V^{k-1}\frac{t^{k-1}}{(k-1)!}.
$$

The series for $Q$ therefore converges uniformly on $[0,T]\times M\times M$. Derivatives obey analogous bounds, with polynomial factors in $k$, by the quoted residual extension and differentiation properties. Thus the series can be convolved and differentiated as above. Associativity and absolute convergence give $Q+R+R*Q=0$, proving $(\partial_t+\Delta_x)H=0$. The correction $P*Q$ has integral norm $O(t)$ by the integral bound on $P$ and boundedness of $Q$. It has zero initial limit, so $H$ has precisely the required delta initial data.

For uniqueness, a smooth solution $w$ with zero initial data satisfies the [heat equation energy identity](../../../../../heat-equation-energy-identity.md)

$$
\frac{d}{dt}\|w(t)\|_{L^2}^2=-2\langle w,\Delta w\rangle=-2\|dw\|_{L^2}^2\le0.
$$

Its initial norm is zero, hence $w=0$. Applying uniqueness to consecutive evolutions proves the [semigroup property](../../../../../semigroup-property.md). Choose $s_0<T$ and, for arbitrary $t>0$, compose enough kernels $H(t/r)$ that $t/r<s_0$. The resulting kernel is independent of the subdivision by uniqueness, is smooth for positive time by the quoted differentiability property, and extends the construction to every $t>0$. This proves **a parametrix determines the global heat kernel** in the closed setting. The [heat equation maximum principle](../../../../../heat-equation-maximum-principle.md) gives nonnegativity and applying uniqueness to the constant initial function gives conservation of total mass. Self-adjointness of the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md) $\Delta$ gives symmetry.

Finally let $\{\phi_j\}$ be a complete complex [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) of $\Delta$, with [eigenvalues](../../../../../eigenvalue.md) $\lambda_j\ge0$, repeated by multiplicity. As subsidiary analytic facts we use the compact elliptic [compact elliptic spectral theorem](../../../../../compact-elliptic-spectral-theorem.md), [elliptic regularity](../../../../../elliptic-regularity.md) bounds making each fixed derivative of $\phi_j$ grow at most polynomially in $1+\lambda_j$, and a polynomial eigenvalue-counting bound. The [spectral expansion of the Riemannian heat kernel](../../../../../spectral-expansion-of-the-riemannian-heat-kernel.md) converges because exponential decay makes the following series converge with every derivative when $t\ge\varepsilon>0$:

$$
\boxed{H(t,x,y)=\sum_{j=0}^{\infty}e^{-t\lambda_j}\phi_j(x)\overline{\phi_j(y)}.}
$$

Indeed, evolving initial data $\phi_j$ gives $e^{-t\lambda_j}\phi_j$ by direct substitution into the [heat equation](../../../../../heat-equation.md) and uniqueness. For general $f\in L^2(M)$, completeness and the [heat equation energy identity](../../../../../heat-equation-energy-identity.md) give

$$
\nu(t,x)=\sum_j e^{-t\lambda_j}\langle f,\phi_j\rangle\phi_j(x).
$$

The smoothly convergent kernel series represents this same operator, and equality for all smooth $f$ identifies it pointwise with the constructed [heat kernel](../../../../../heat-kernel.md). The complex conjugate is required by the [inner product](../../../../../inner-product.md); for a real [eigenbasis](../../../../../eigenbasis.md) it may be omitted. A noncompact [Riemannian manifold](../../../../../riemannian-manifold.md) may instead require a spectral integral, and the unqualified discrete formula should not be asserted there.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
