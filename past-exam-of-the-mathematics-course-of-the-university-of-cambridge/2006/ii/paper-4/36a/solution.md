<h1 id="36a/solution">Solution</h1>

↑ **Parent:** [36A](../36a.md)

[Normal coordinates](../../../../../normal-coordinates.md) at an event have $g_{ab}=\eta_{ab}$ and first metric derivatives, equivalently connection coefficients, zero there. They describe freely falling frames in which nongravitational laws take their special-relativistic form to first order, expressing the [Equivalence principle](../../../../../equivalence-principle.md). Curvature and tidal effects cannot generally be removed throughout a neighbourhood.

For a covector, $\nabla_aV_b=\partial_aV_b-\Gamma^c_{ab}V_c$. The [Levi-Civita connection](../../../../../levi-civita-connection.md) is torsion-free, so

$$
\partial_aV_b-\partial_bV_a=\nabla_aV_b-\nabla_bV_a
$$

is an antisymmetric [covariant tensor](../../../../../covariant-tensor.md). Next expand $\nabla_aK_b+\nabla_bK_a$ using $K_b=g_{bc}K^c$ and $2g_{cd}\Gamma^d_{ab}=\partial_ag_{bc}+\partial_bg_{ac}-\partial_cg_{ab}$. Cancelling the first two metric derivatives leaves

$$
\boxed{2\nabla_{(a}K_{b)}=K^c\partial_cg_{ab}+g_{ac}\partial_bK^c+g_{bc}\partial_aK^c=Q_{ab}}.
$$

If $K=\partial_4$ has constant coordinate components, $Q_{ab}=\partial_4g_{ab}$. Thus $Q=0$ implies the metric is independent of $x^4$ and $K$ is a [Killing vector](../../../../../killing-vector-field.md). Its derivative is antisymmetric, yielding

$$
\boxed{\nabla_aK_b=\tfrac12(\partial_aK_b-\partial_bK_a)}.
$$

For an affinely parametrized [geodesic](../../../../../geodesic.md) with tangent $u$, differentiation gives

$$
\frac d{d\lambda}(-K_au^a)=-u^au^b\nabla_aK_b-K_a\nabla_uu^a=0.
$$

The first term vanishes by antisymmetry and the second by the [geodesic equation](../../../../../geodesic-equation.md), proving conservation in every coordinate system. A stationary metric requires the [Killing vector](../../../../../killing-vector-field.md) to be timelike in the region concerned. For particle energy, the tangent should be future timelike for a massive particle, with affine parameter proportional to [proper time](../../../../../proper-time.md), or future null with appropriate momentum normalization for a [photon](../../../../../photon.md); normalize the future timelike [Killing vector](../../../../../killing-vector-field.md) relative to the chosen stationary observers or at infinity. Then the conserved quantity is proportional to their Killing energy. A spacelike [Killing vector](../../../../../killing-vector-field.md) instead represents momentum, not stationary time translation.

## ↑ Ancestors (10)

1. [36A](../36a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
