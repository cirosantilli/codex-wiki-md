<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [cotangent space](../../../../../../cotangent-space.md) $T_p^*M=\operatorname{Hom}_{\mathbb R}(T_pM,\mathbb R)$ and the [cotangent bundle](../../../../../../cotangent-bundle.md) $T^*M=\coprod_pT_p^*M$, with projection $(p,\alpha)\mapsto p$. A [coordinate chart](../../../../../../manifold-chart.md) $x$ gives the dual [basis](../../../../../../basis.md) $dx^1|_p,\ldots,dx^n|_p$. Write $\alpha=\sum_i\xi_i dx^i|_p$ and define the induced [local trivialization](../../../../../../local-trivialization.md) by

$$
\Psi_x(p,\alpha)=(x(p),\xi)\in x(U)\times\mathbb R^n.
$$

If $y=f(x)$ and $\alpha=\sum_j\eta_jdy^j$, the [chain rule](../../../../../../chain-rule.md) gives $\xi=D f(x)^T\eta$. Therefore the [cotangent coordinate transition](../../../../../../cotangent-coordinate-transition.md) is

$$
\boxed{\Psi_y\Psi_x^{-1}(z,\xi)=(f(z),D f(z)^{-T}\xi).}
$$

The inverse [Jacobian matrix](../../../../../../jacobian-matrix.md) is smooth wherever its determinant is nonzero, so this transition and its inverse are smooth. The cocycle follows either from the chain rule or by dualizing the tangent transitions.

Use these product charts to define the topology and smooth atlas. The [Hausdorff](../../../../../../hausdorff-space.md) and second-countability arguments are the same as for the [tangent bundle](../../../../../../tangent-bundle.md): separate distinct fibres using the base, separate distinct [covectors](../../../../../../covector.md) in one product chart, and use a countable coordinate cover. The fibre transitions are smooth linear isomorphisms, so the projection is a smooth [vector bundle](../../../../../../vector-bundle.md) of rank $n$. Using every compatible base [coordinate chart](../../../../../../manifold-chart.md) shows that this structure is natural and independent of chart choices.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
