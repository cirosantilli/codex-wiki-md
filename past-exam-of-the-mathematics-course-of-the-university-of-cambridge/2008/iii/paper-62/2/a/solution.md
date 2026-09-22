<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathcal L=-\tfrac12g^{\alpha\beta}\partial_\alpha\phi\partial_\beta\phi-V$. In the [metric variation](../../../../../../metric-variation.md) specified here, the covariant [metric tensor](../../../../../../metric-tensor.md) $g_{\mu\nu}$ is varied while the [scalar field](../../../../../../scalar-field.md) is held fixed. Differentiating the inverse and the determinant gives

$$
\delta g^{\alpha\beta}=-g^{\alpha\mu}g^{\beta\nu}\delta g_{\mu\nu},\qquad
\delta\sqrt{-g}=\frac12\sqrt{-g}\,g^{\mu\nu}\delta g_{\mu\nu}.
$$

Thus $\delta\mathcal L=\tfrac12\partial^\mu\phi\partial^\nu\phi\,\delta g_{\mu\nu}$, and the [action](../../../../../../action.md) varies as

$$
\delta S_M=\frac12\int d^4x\sqrt{-g}
\left(\partial^\mu\phi\partial^\nu\phi+g^{\mu\nu}\mathcal L\right)\delta g_{\mu\nu}.
$$

The functional derivative therefore gives $T^{\mu\nu}=\partial^\mu\phi\partial^\nu\phi+g^{\mu\nu}\mathcal L$. Lowering both indices yields the [stress-energy tensor of a canonical scalar field](../../../../../../stress-energy-tensor-of-a-canonical-scalar-field.md):

$$
\boxed{T_{\mu\nu}=\partial_\mu\phi\partial_\nu\phi
-g_{\mu\nu}\left(\frac12g^{\alpha\beta}\partial_\alpha\phi\partial_\beta\phi+V\right).}
$$

The determinant variation has a positive sign because the variable is $g_{\mu\nu}$; varying the inverse [metric tensor](../../../../../../metric-tensor.md) instead would reverse that intermediate sign.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
