# Coercive weak formulation of a coupled Dirichlet-Neumann system

↑ **Parent:** [Lax-Milgram theorem](lax-milgram-theorem.md)

For $H=H_0^1(U)\times H^1(U)$, the coupled form

$$
B((u,w),(v,z))=\int_U\bigl(Du\mathbin\cdot Dv+uv+wv+Dw\mathbin\cdot Dz+wz-3uz\bigr)
$$

satisfies

$$
B((u,w),(u,w))=\|Du\|_2^2+\|Dw\|_2^2+\|u-w\|_2^2.
$$

The [Poincaré inequality](poincare-inequality.md) for $u$ then controls both $\|u\|_2$ and $\|w\|_2$, so the form is [coercive](coercive-bilinear-form.md) on $H$. The [Lax-Milgram theorem](lax-milgram-theorem.md) therefore gives a unique [weak solution](weak-solution.md). The first component has a [Dirichlet boundary condition](dirichlet-boundary-condition.md), while the second component's [Neumann boundary condition](neumann-boundary-condition.md) is the natural boundary condition in the [weak formulation](weak-formulation.md).

## ↑ Ancestors (6)

1. [Lax-Milgram theorem](lax-milgram-theorem.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
