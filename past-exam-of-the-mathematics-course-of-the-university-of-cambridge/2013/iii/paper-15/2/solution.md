<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [Riemannian metric](../../../../../riemannian-metric.md) is a smooth field of positive-definite [symmetric bilinear forms](../../../../../symmetric-bilinear-form.md) $g_x$ on the [tangent spaces](../../../../../tangent-space.md), equivalently a smooth section of $\operatorname{Sym}^2T^*M$ with that positivity. Its [musical isomorphism](../../../../../musical-isomorphism.md) is

$$
\boxed{\flat_g:TM\longrightarrow T^*M,\qquad v\longmapsto g(v,\cdot)}.
$$

Nondegeneracy makes every fiber map an isomorphism. In coordinates the map has matrix $g_{ij}$, and its inverse $\sharp_g$ has matrix $g^{ij}$. Smoothness of the inverse follows from the inverse-matrix formula and the nonvanishing [determinant](../../../../../determinant.md). Both maps cover the identity on $M$, giving a smooth [vector bundle isomorphism](../../../../../vector-bundle-isomorphism.md).

For [local flattening of a Riemannian metric](../../../../../local-flattening-of-a-riemannian-metric.md), choose a [manifold chart](../../../../../manifold-chart.md) neighborhood $V$ around $p$ with closure contained in $U$, and let $h=\phi^*\delta$ on $V$. Choose a [smooth bump function](../../../../../smooth-bump-function.md) $0\leq\chi\leq1$, with [compact support](../../../../../compact-support.md) in $V$ and equal to one on a smaller neighborhood $W$ of $p$. Set

$$
\boxed{\widetilde g=(1-\chi)g+\chi h\text{ on }V,\qquad\widetilde g=g\text{ off }V}.
$$

The formulas glue smoothly because the modification is supported strictly inside $V$. A convex combination of positive-definite forms is positive definite. On $W$ the metric is exactly $h$, so $\phi$ gives an [isometry](../../../../../isometry.md) to a Euclidean open subset. Outside $U$ the original metric remains unchanged.

[Geodesic completeness](../../../../../geodesic-completeness.md) means that every [geodesic](../../../../../geodesic.md) with arbitrary initial point and tangent vector extends for every real affine parameter. On each [connected](../../../../../connected-space.md) component, the [Hopf-Rinow theorem](../../../../../hopf-rinow-theorem.md) equates this with completeness of the [Riemannian distance](../../../../../riemannian-distance.md).

The Euclidean-end claim needs a compact-core interpretation that is absent from its literal hypotheses. Indeed, $M=\{x\in\mathbb R^n:|x|>1\}$ with $n\geq2$, $X=\varnothing$ and $g=\delta$ satisfy those hypotheses. The [geodesic](../../../../../geodesic.md) $\gamma(t)=(2-t)e_1$ reaches the missing unit sphere at $t=1$ and cannot continue within $M$. Thus the printed assumptions alone do not prove completeness.

Here is the intended [compact-core completeness for a Euclidean end](../../../../../compact-core-completeness-for-a-euclidean-end.md). Write $\Phi:M\setminus X\to\{|x|>1\}$ for the end coordinates and assume additionally that

$$
K_R=X\cup\Phi^{-1}\{1<|x|\leq R\}
$$

is [compact](../../../../../compact-space.md) for every sufficiently large $R$. Choose such an $R$ beyond the metric transition and large enough to include the initial point of a [geodesic](../../../../../geodesic.md). Its speed $s$ is constant. On every segment outside $K_R$, the Euclidean radius changes at a rate at most $s$, so over a finite parameter interval it cannot exceed $R+sT$. The full segment therefore stays in the [compact](../../../../../compact-space.md) set $K_{R+sT}$. Its velocities also stay in a [compact](../../../../../compact-space.md) subset of $TM$, since their metric [norm](../../../../../norm.md) is fixed and the base set is [compact](../../../../../compact-space.md). The smooth [geodesic](../../../../../geodesic.md) ordinary differential equation consequently extends past any supposed finite endpoint. The reversed-time argument is identical. This proves completeness under the compact-core condition, and explains exactly what the exterior-of-a-ball counterexample lacks.

For [upward stability of Riemannian completeness](../../../../../upward-stability-of-riemannian-completeness.md), lengths of all curves satisfy $L_{\widetilde g}\geq L_g$, hence $d_{\widetilde g}\geq d_g$. A $d_{\widetilde g}$-Cauchy sequence is therefore $d_g$-Cauchy and has a limit $p$ because $g$ is complete. Smooth positive-definite metrics induce the manifold topology. More explicitly, on a small coordinate ball around $p$, $\widetilde g$ has a bounded largest matrix [eigenvalue](../../../../../eigenvalue.md), so the coordinate straight segment gives $d_{\widetilde g}(p,q)\leq C|\phi(q)-\phi(p)|$. Thus convergence to $p$ is also in $d_{\widetilde g}$. That distance is complete, and Hopf-Rinow yields

$$
\boxed{\widetilde g\geq g,\quad g\text{ complete}\quad\Longrightarrow\quad\widetilde g\text{ complete}}.
$$

For disconnected $M$, apply this argument on each component.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
