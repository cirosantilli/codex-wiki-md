<h1 id="23h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $H=H_0^1(\Omega)$ with its usual [Hilbert space](../../../../../../hilbert-space-split.md) inner product, and define

$$
B(u,v)=\int_\Omega\left(\nabla u\mathbin\cdot\nabla v+uv+uA\mathbin\cdot\nabla v\right).
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) shows that this is a [bounded bilinear form](../../../../../../bounded-bilinear-form.md). For $u\in H$, [Young inequality](../../../../../../young-s-inequality-for-products.md) gives

$$
\left|\int_\Omega uA\mathbin\cdot\nabla u\right|
\leq |A|_2\lVert u\rVert_2\lVert\nabla u\rVert_2
\leq\frac{|A|_2}{2}\left(\lVert u\rVert_2^2+\lVert\nabla u\rVert_2^2\right),
$$

and therefore

$$
B(u,u)\geq\left(1-\frac{|A|_2}{2}\right)\lVert u\rVert_{H^1}^2.
$$

Because $|A|_2<2$, this is a [coercive bilinear form](../../../../../../coercive-bilinear-form.md).

The map $u\mapsto\int_\Omega uf$ is a [bounded linear functional](../../../../../../continuous-linear-functional.md) on $H$. By the [Riesz representation theorem](../../../../../../riesz-representation-theorem.md), it equals $\langle u,F\rangle_H$ for some $F\in H$. Applying part (b) produces one and only one $v\in H$ such that

$$
\boxed{\int_\Omega\left(\nabla u\mathbin\cdot\nabla v+uv+uA\mathbin\cdot\nabla v\right)=\int_\Omega uf
\quad\text{for every }u\in H_0^1(\Omega).}
$$

This is precisely the [weak formulation](../../../../../../weak-formulation.md) of the stated [Dirichlet problem](../../../../../../dirichlet-problem.md), obtained by [integration by parts](../../../../../../integration-by-parts.md) in the [Laplace operator](../../../../../../laplace-operator.md) term. Thus $v$ is its unique [weak solution](../../../../../../weak-solution.md); this is the [constant-drift massive-Laplacian Dirichlet problem](../../../../../../constant-drift-massive-laplacian-dirichlet-problem.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [23H](../../23h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
