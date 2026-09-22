<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Dirichlet boundary condition](../../../../../../../dirichlet-boundary-condition.md) is built into the first component's space, while the [Neumann boundary condition](../../../../../../../neumann-boundary-condition.md) is natural. Thus a [weak solution](../../../../../../../weak-solution.md) is a pair

$$
(u,w)\in H_0^1(U)\times H^1(U)
$$

such that for every $(v,z)\in H_0^1(U)\times H^1(U)$,

$$
\int_U(Du\mathbin\cdot Dv+uv+wv)=\int_Ufv,
$$



$$
\int_U(Dw\mathbin\cdot Dz+wz-3uz)=\int_Ugz.
$$

If $u,w$ are $C^2$ up to the boundary, taking compactly supported [test functions](../../../../../../../test-function.md) and applying the [fundamental lemma of the calculus of variations](../../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives both differential equations pointwise in $U$. Membership of $H_0^1(U)$ gives $u=0$ on $\partial U$. Applying [integration by parts](../../../../../../../integration-by-parts.md) to the second identity and using its differential equation leaves

$$
\int_{\partial U}\frac{\partial w}{\partial\nu}z=0
$$

for every smooth boundary trace $z$. Hence $\partial w/\partial\nu=0$ on $\partial U$, so the equations and both boundary conditions hold classically.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
