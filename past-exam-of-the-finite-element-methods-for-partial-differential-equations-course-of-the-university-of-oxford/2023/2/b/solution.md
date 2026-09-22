<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Sobolev space with a partial Dirichlet condition](../../../../sobolev-space-with-a-partial-dirichlet-condition.md)

$$
\boxed{V=\{v\in H^1(\Omega):Tv=0\text{ almost everywhere on }\Gamma_D\},}
$$

where $T$ is the [Sobolev trace operator](../../../../trace-operator.md). The restricted [Sobolev trace operator](../../../../trace-operator.md) is continuous into $L^2(\Gamma_D)$; its [kernel](../../../../kernel-of-a-linear-map-split.md) is consequently a [closed vector subspace](../../../../closed-vector-subspace.md) of $H^1(\Omega)$. Thus $V$, with the first-order [Sobolev norm](../../../../sobolev-norm.md), is a [Hilbert space](../../../../hilbert-space-split.md). The endpoint convention for $\Gamma_D$ and $\Gamma_N$ does not affect this definition: finitely many boundary points have zero boundary length. It would be inappropriate to impose pointwise boundary values on arbitrary $H^1$ functions in two dimensions.

For a smooth solution, [Green's first identity](../../../../green-s-first-identity.md) gives

$$
\int_\Omega(-\Delta u+u)v
=\int_\Omega(\nabla u\cdot\nabla v+uv)-\int_{\partial\Omega}\partial_nu\,Tv.
$$

The boundary term vanishes because $Tv=0$ on $\Gamma_D$ and the [normal derivative](../../../../normal-derivative.md) is zero on $\Gamma_N$. This suggests the [weak formulation](../../../../weak-formulation.md)

$$
\boxed{u\in V,\qquad a(u,v)=\ell(v)\quad(v\in V),\qquad
a(p,v)=(\nabla p,\nabla v)_0+(p,v)_0,\quad\ell(v)=(f,v)_0.}
$$

Here $a$ is exactly the first-order [Sobolev inner product](../../../../sobolev-inner-product.md). In particular the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) gives

$$
|a(p,v)|\leq\|p\|_1\|v\|_1,\qquad a(v,v)=\|v\|_1^2,\qquad
|\ell(v)|\leq\|f\|_0\|v\|_1.
$$

Thus $a$ is a [bounded bilinear form](../../../../bounded-bilinear-form.md) and a [coercive bilinear form](../../../../coercive-bilinear-form.md), both with constant one. The [Lax-Milgram theorem](../../../../lax-milgram-theorem.md) proves existence and uniqueness, together with

$$
\boxed{\|u\|_1\leq\|f\|_0.}
$$

The positive reaction term already controls the entire [Sobolev norm](../../../../sobolev-norm.md), so no [Poincaré inequality](../../../../poincare-inequality.md) is needed here. The zero [Neumann boundary condition](../../../../neumann-boundary-condition.md) is the natural part of the [weak formulation](../../../../weak-formulation.md); it is not an additional restriction on the test space. For this [weak solution](../../../../weak-solution.md), $-\Delta u+u=f$ holds as a [distributional identity](../../../../distributional-identity.md), and the zero [normal derivative](../../../../normal-derivative.md) on $\Gamma_N$ is understood through the corresponding [Green's first identity](../../../../green-s-first-identity.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
