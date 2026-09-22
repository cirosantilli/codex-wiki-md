<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Contract the printed [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) using $R_{ab}=R^\mu{}_{a\mu b}$. Only the derivative terms can contain second derivatives of the [metric tensor](../../../../../../metric-tensor.md):

$$
R_{ab}=\partial_\mu\Gamma^\mu{}_{ab}-\partial_b\Gamma^\mu{}_{a\mu}
+\Gamma^\tau{}_{ab}\Gamma^\mu{}_{\tau\mu}-\Gamma^\tau{}_{a\mu}\Gamma^\mu{}_{\tau b}.
$$

Substituting the [Christoffel symbol](../../../../../../christoffel-symbol.md) formula, its second derivative part is

$$
\frac12g^{\mu\nu}\left(\partial_\mu\partial_a g_{\nu b}+\partial_\mu\partial_b g_{\nu a}
-\partial_\mu\partial_\nu g_{ab}-\partial_a\partial_b g_{\mu\nu}\right).
$$

Set $H_b=g_{b\lambda}H^\lambda=g^{\mu\nu}\partial_\mu g_{\nu b}-\tfrac12g^{\mu\nu}\partial_b g_{\mu\nu}$. The first, second and fourth terms are the second derivative terms of $\tfrac12(\partial_aH_b+\partial_bH_a)$. Derivatives of the inverse [metric tensor](../../../../../../metric-tensor.md) produce only products of first derivatives. Thus

$$
R_{ab}=-\frac12g^{\mu\nu}\partial_\mu\partial_\nu g_{ab}
+\frac12(\partial_aH_b+\partial_bH_a)+Q_{ab}(g,\partial g),
$$

where $Q$ contains at most first metric derivatives. In [harmonic coordinates](../../../../../../harmonic-coordinate.md), $H^\lambda$ vanishes throughout the chart, so $H_b$ and its derivatives vanish. **The vacuum equations have the wave principal part**

$$
\boxed{R_{ab}=-\frac12g^{\mu\nu}\partial_\mu\partial_\nu g_{ab}+Q_{ab}(g,\partial g)=0.}
$$

These are [quasilinear partial differential equations](../../../../../../quasilinear-partial-differential-equation.md) with the principal part of a [wave equation](../../../../../../wave-equation-split.md), because $g^{\mu\nu}$ has Lorentzian signature. This is the [harmonic reduction of the vacuum Einstein equations](../../../../../../harmonic-reduction-of-the-vacuum-einstein-equations.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
