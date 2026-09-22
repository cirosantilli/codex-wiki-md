<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [canonical momentum](../../../../../../canonical-momentum.md) equation is $\dot X=eP+uX'$. Eliminating $P$ from the [phase-space action](../../../../../../phase-space-action.md) yields the [Lagrangian density](../../../../../../lagrangian-density.md)

$$
\mathcal L=\frac{(\dot X-uX')^2}{2e}-\frac{eT^2}{2}X'^2.
$$

This is the [Polyakov action](../../../../../../polyakov-action.md) after identifying its inverse [metric tensor](../../../../../../metric-tensor.md) density as

$$
\sqrt{-\gamma}\,\gamma^{\mu\nu}
=\frac1{Te}\begin{pmatrix}-1&u\\u&T^2e^2-u^2\end{pmatrix},\qquad
\gamma=\det\gamma_{\mu\nu}.
$$

The [determinant](../../../../../../determinant.md) of this [matrix](../../../../../../matrix.md) is $-1$, as required in two dimensions. The [Weyl transformation](../../../../../../weyl-transformation.md) leaves the [matrix](../../../../../../matrix.md) unchanged, so $e,u$ encode the metric modulo its [conformal factor](../../../../../../conformal-factor.md).

Define the [induced worldsheet metric](../../../../../../induced-worldsheet-metric.md) by $g_{\mu\nu}=\eta_{mn}\partial_\mu X^m\partial_\nu X^n$. Varying the independent inverse [metric tensor](../../../../../../metric-tensor.md) in the [Polyakov action](../../../../../../polyakov-action.md) gives

$$
g_{\mu\nu}-\tfrac12\gamma_{\mu\nu}\gamma^{\rho\sigma}g_{\rho\sigma}=0.
$$

Consequently $g_{\mu\nu}=f\gamma_{\mu\nu}$, where $f=\tfrac12\gamma^{\rho\sigma}g_{\rho\sigma}$. For a nondegenerate Lorentzian [string worldsheet](../../../../../../worldsheet.md) with the usual compatible time orientation, take $f>0$, or $\gamma_{\mu\nu}=e^{2\omega}g_{\mu\nu}$. The undetermined function is precisely [Weyl invariance](../../../../../../weyl-transformation.md). Since $\sqrt{-\gamma}\,\gamma^{\mu\nu}g_{\mu\nu}=2\sqrt{-g}$, elimination of the independent [metric tensor](../../../../../../metric-tensor.md) gives

$$
\boxed{I_{\mathrm{NG}}=-T\int dt\,d\sigma\,\sqrt{-\det g_{\mu\nu}}.}
$$

Thus the [Nambu–Goto action](../../../../../../nambu-goto-action.md) measures minus [string tension](../../../../../../string-tension.md) times Lorentzian [worldsheet area](../../../../../../worldsheet-area.md). The metric elimination holds in the nondegenerate interior; null endpoints are understood as boundary limits.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
