<h1 id="36b/solution">Solution</h1>

↑ **Parent:** [36B](../36b.md)

Use metric compatibility and the symmetric [Levi-Civita connection](../../../../../levi-civita-connection.md). Expanding $k_a=g_{ac}k^c$ gives

$$
\nabla_bk_a+\nabla_ak_b
=g_{ac}\partial_bk^c+g_{bc}\partial_ak^c+
k^c(\partial_bg_{ac}+\partial_ag_{bc}-2\Gamma^d_{ab}g_{dc}).
$$

The Christoffel formula makes the bracket $\partial_cg_{ab}$. Thus the [Killing equation](../../../../../killing-equation.md) is equivalent to the displayed coordinate formula in the question, also the vanishing [Lie derivative](../../../../../lie-derivative-of-a-differential-form.md) of the metric.

Along an affinely parametrized [geodesic](../../../../../geodesic.md) with tangent $V$,

$$
V^b\nabla_b(V^ak_a)=k_aV^b\nabla_bV^a+V^aV^b\nabla_bk_a=0.
$$

The first term vanishes by the geodesic equation and the second by the Killing equation, because $V^aV^b$ is symmetric. This proves the [geodesic conserved quantity from a Killing vector](../../../../../geodesic-conserved-quantity-from-a-killing-vector.md).

For $ds^2=-du^2+u^2dv^2$, the three independent coordinate Killing conditions are

$$
\partial_uk^u=0,\qquad uk^u+u^2\partial_vk^v=0,\qquad-\partial_vk^u+u^2\partial_uk^v=0.
$$

The field $(0,1)$ satisfies all three immediately. For $e^{-v}(1,u^{-1})$, the second equation reads $ue^{-v}-ue^{-v}=0$, and the third reads $e^{-v}-e^{-v}=0$. For $e^v(-1,u^{-1})$, they read $-ue^v+ue^v=0$ and $e^v-e^v=0$. The first equation holds for both, verifying all three [Killing vector fields](../../../../../killing-vector-field.md).

Their conserved contractions with $(\dot u,\dot v)$ may be denoted

$$
\gamma=u^2\dot v,\qquad
\alpha=e^{-v}(-\dot u+u\dot v),\qquad
\beta=e^v(\dot u+u\dot v).
$$

Adding the last two expressions after multiplying by $e^v,e^{-v}$ gives

$$
\boxed{\alpha e^v+\beta e^{-v}=2\gamma/u}.
$$

To identify these loci, set $T=u\cosh v$, $X=u\sinh v$. The metric becomes $-dT^2+dX^2$, and the equation becomes $(\alpha+\beta)T+(\alpha-\beta)X=2\gamma$, a straight line in [Minkowski spacetime](../../../../../minkowski-spacetime.md). Nontrivial such lines, parametrized affinely, are exactly the geodesics in this coordinate patch. The all-zero choice of constants is a vacuous equation rather than an individual geodesic.

## ↑ Ancestors (10)

1. [36B](../36b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
