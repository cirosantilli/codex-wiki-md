# Skew-coupled elliptic system

↑ **Parent:** [Elliptic boundary value problem](elliptic-boundary-value-problem-split.md)

A [skew-coupled elliptic system](skew-coupled-elliptic-system.md) has zeroth-order couplings with opposite signs. For the displayed example with homogeneous [Dirichlet boundary conditions](dirichlet-boundary-condition.md), its [weak formulation](weak-formulation.md) on $V=H_0^1(\Omega)\times H_0^1(\Omega)$ has the [bilinear form](bilinear-form-split.md)

$$
b((p,q),(v,z))=(\nabla p,\nabla v)_0+(\nabla q,\nabla z)_0-(q,v)_0+(p,z)_0.
$$

The coupling cancels for equal arguments, so $b((p,q),(p,q))=\|\nabla p\|_0^2+\|\nabla q\|_0^2$. On a domain satisfying the [Poincaré inequality](poincare-inequality.md), this is a [coercive bilinear form](coercive-bilinear-form.md). With the product first-order [Sobolev norm](sobolev-norm.md), the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) applied to $(\nabla p,\nabla q,-q,p)$ and $(\nabla v,\nabla z,v,z)$ gives $|b(P,T)|\leq\|P\|_V\|T\|_V$. The [Lax-Milgram theorem](lax-milgram-theorem.md) therefore applies even though the [bilinear form](bilinear-form-split.md) is not symmetric. Eliminating $w=-\Delta u$ recovers $\Delta^2u+u=f$, involving the [biharmonic operator](biharmonic-operator.md).

## ↑ Ancestors (6)

1. [Elliptic boundary value problem](elliptic-boundary-value-problem-split.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/1/a/solution.md)
- [Solution](past-exam-of-the-finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford/2023/1/b/solution.md)
- [Skew-coupled elliptic system](skew-coupled-elliptic-system.md)
