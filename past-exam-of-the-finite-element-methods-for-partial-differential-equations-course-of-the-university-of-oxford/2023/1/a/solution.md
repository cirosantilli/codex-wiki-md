<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a sufficiently regular solution, put $w=-\Delta u$, with $\Delta$ the [Laplacian](../../../../laplacian.md). Then $-\Delta u-w=0$ and $u-\Delta w=u+\Delta^2u=f$. The zero [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) on $u$ and $\Delta u$ become zero [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) on $u$ and $w$. Conversely, eliminating $w$ from these two equations recovers the fourth-order equation with the [biharmonic operator](../../../../biharmonic-operator.md). For the [weak solution](../../../../weak-solution.md) we will construct, these interior identities hold as [distributional identities](../../../../distributional-identity.md); zero [Sobolev traces](../../../../trace-operator.md) are imposed on $u$ and $w$, without assuming classical fourth [derivatives](../../../../derivative.md) of $u$.

Let $V=H_0^1(\Omega)\times H_0^1(\Omega)$, the [Cartesian product](../../../../cartesian-product.md) of two [zero-boundary Sobolev spaces](../../../../zero-boundary-sobolev-space.md), with [norm](../../../../norm.md)

$$
\|(p,q)\|_V^2=\|p\|_1^2+\|q\|_1^2.
$$

This is a [Hilbert space](../../../../hilbert-space-split.md). Applying [integration by parts](../../../../integration-by-parts.md) separately to the two equations gives the [weak formulation](../../../../weak-formulation.md)

$$
\boxed{\begin{aligned}
(\nabla u,\nabla v)_0-(w,v)_0&=0&&\text{for every }v\in H_0^1(\Omega),\\
(u,z)_0+(\nabla w,\nabla z)_0&=(f,z)_0&&\text{for every }z\in H_0^1(\Omega).
\end{aligned}}
$$

Equivalently, for $U=(u,w)$ and $T=(v,z)$, define the [bilinear form](../../../../bilinear-form-split.md) and [linear functional](../../../../linear-functional.md)

$$
\begin{aligned}
b((p,q),(v,z))&=(\nabla p,\nabla v)_0+(\nabla q,\nabla z)_0-(q,v)_0+(p,z)_0,\\
F(v,z)&=(f,z)_0.
\end{aligned}
$$

We seek $U\in V$ with $b(U,T)=F(T)$ for every $T\in V$.

The [skew-coupled elliptic system](../../../../skew-coupled-elliptic-system.md) has a useful [bounded bilinear form](../../../../bounded-bilinear-form.md) estimate with constant one. Indeed, write the [integrand](../../../../integrand.md) as the [dot product](../../../../dot-product.md) of $(\nabla p,\nabla q,-q,p)$ and $(\nabla v,\nabla z,v,z)$. The [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) gives

$$
|b((p,q),(v,z))|\leq\|(p,q)\|_V\|(v,z)\|_V,
\qquad |F(v,z)|\leq\|f\|_0\|(v,z)\|_V.
$$

For equal arguments, the two zeroth-order coupling terms cancel. If $K$ is the constant in the supplied [Poincaré inequality](../../../../poincare-inequality.md), then

$$
b((p,q),(p,q))=\|\nabla p\|_0^2+\|\nabla q\|_0^2
\geq\frac1{1+K}\|(p,q)\|_V^2.
$$

Thus $b$ is a [coercive bilinear form](../../../../coercive-bilinear-form.md), although it is not a [symmetric bilinear form](../../../../symmetric-bilinear-form.md). The [Lax-Milgram theorem](../../../../lax-milgram-theorem.md) applies and yields

$$
\boxed{\text{There is exactly one }(u,w)\in H_0^1(\Omega)\times H_0^1(\Omega)\text{ solving the weak system.}}
$$

In particular, $\|(u,w)\|_V\leq(1+K)\|f\|_0$. Testing with compactly supported smooth [test functions](../../../../test-function.md) identifies $-\Delta u=w$ and $-\Delta w=f-u$ as [distributional identities](../../../../distributional-identity.md). This gives the asserted relation to the original [boundary value problem](../../../../boundary-value-problem-split.md) at the available regularity.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the finite element methods for partial differential equations course of the University of Oxford](../../../split.md)
5. [Finite element methods for partial differential equations course of the University of Oxford](../../../../finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
