# Korn inequality

↑ **Parent:** [Sobolev space](sobolev-space-split.md)

The zero-boundary [Korn inequality](korn-inequality.md) controls the full [displacement gradient tensor](displacement-gradient-tensor.md) by the [infinitesimal strain tensor](infinitesimal-strain-tensor.md) for $v\in H_0^1(\Omega;\mathbb R^d)$. On a bounded [Lipschitz domain](lipschitz-domain.md), combining it with the [Poincaré inequality](poincare-inequality.md) makes a positive [linear elasticity](linear-elasticity.md) energy a [coercive bilinear form](coercive-bilinear-form.md) in the first-order [Sobolev norm](sobolev-norm.md). The zero [Dirichlet boundary condition](dirichlet-boundary-condition.md) removes the otherwise uncontrolled rigid displacements.

For this zero-boundary version one can prove an exact identity. For a smooth compactly supported [vector field](vector-field.md), two applications of [integration by parts](integration-by-parts.md) give

$$
\sum_{i,j}\int_\Omega\partial_jv_i\,\partial_iv_j=\int_\Omega(\operatorname{div}v)^2.
$$

Expanding the symmetric gradient and using density in the [zero-boundary Sobolev space](zero-boundary-sobolev-space.md) therefore yields

$$
2\|\varepsilon(v)\|_{L^2}^2=\|\nabla v\|_{L^2}^2+\|\operatorname{div}v\|_{L^2}^2.
$$

In three dimensions this also gives the stronger trace-free version

$$
\left\|\varepsilon(v)-\frac13(\operatorname{div}v)I\right\|_{L^2}^2=\frac12\|\nabla v\|_{L^2}^2+\frac16\|\operatorname{div}v\|_{L^2}^2\geq\frac12\|\nabla v\|_{L^2}^2.
$$

Here the matrix-valued [L2 norm](l2-norm.md) uses the [Frobenius inner product](frobenius-inner-product.md). This explains why the trace-free form printed in the examination suffices for the usual [Korn inequality](korn-inequality.md) estimate.

## ↑ Ancestors (6)

1. [Sobolev space](sobolev-space-split.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Korn inequality](korn-inequality.md)
- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/3/a/solution.md)
- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/3/b/solution.md)
