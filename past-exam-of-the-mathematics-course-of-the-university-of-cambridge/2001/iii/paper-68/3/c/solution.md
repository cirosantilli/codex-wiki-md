<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Although [connection coefficients](../../../../../../connection-components.md) are not [tensor](../../../../../../tensor.md) components, their variation $C^a{}_{bc}=\delta\Gamma^a{}_{bc}$ is [tensorial](../../../../../../tensoriality.md): the [difference of affine connections is a tensor](../../../../../../difference-of-affine-connections-is-a-tensor.md). Varying the [Levi-Civita connection](../../../../../../levi-civita-connection.md) at fixed coordinates gives

$$
C^a{}_{bc}=\frac12g^{ad}
(\nabla_b\delta g_{cd}+\nabla_c\delta g_{bd}-\nabla_d\delta g_{bc}).
$$

In the paper's [curvature sign convention](../../../../../../curvature-sign-convention.md), varying the [derivative](../../../../../../derivative.md) and quadratic-connection terms and grouping them into [covariant derivatives](../../../../../../covariant-derivative.md) gives the [Palatini identity](../../../../../../palatini-identity.md)

$$
\boxed{\delta R_{bc}=\nabla_cC^a{}_{ba}-\nabla_aC^a{}_{bc}.}
$$

One may verify the grouping in [normal coordinates](../../../../../../normal-coordinates.md) at a point, where the [affine connection](../../../../../../affine-connection.md) vanishes and the expression is just the difference of two [partial derivatives](../../../../../../partial-derivative.md); both sides are [tensors](../../../../../../tensor.md), so it holds in every [coordinate frame](../../../../../../coordinate-basis.md). Reversing the definition of the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) reverses this identity's right-hand side.

For completeness, put $q_{ab}=\delta g_{ab}$ and $q=g^{ab}q_{ab}$. The contracted variation uses $C^a{}_{ba}=\nabla_bq/2$ and $g^{bc}C^a{}_{bc}=\nabla_bq^{ab}-\nabla^aq/2$. After two [integrations by parts](../../../../../../integration-by-parts.md),

$$
\int\sqrt{-g}\,\Phi g^{bc}\delta R_{bc}\,d^4x
=\int\sqrt{-g}\left[-\nabla_a\nabla_b\Phi\,q^{ab}
+\Box\Phi\,q\right]d^4x,
$$

up to the discarded [boundary term](../../../../../../boundary-term.md). Substituting $q^{ab}=-\delta g^{ab}$ gives the differentiated-scalar terms in the [metric variation of a scalar-curvature coupling](../../../../../../metric-variation-of-a-scalar-curvature-coupling.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
