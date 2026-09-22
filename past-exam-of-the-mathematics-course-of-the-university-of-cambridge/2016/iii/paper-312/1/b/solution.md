<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a dot for the coordinate-time derivative and let $\bar N$ be the homogeneous background [lapse function](../../../../../../lapse-function.md). The passive linear transformation is $\delta\widetilde g_{\mu\nu}=\delta g_{\mu\nu}-\mathcal L_\xi\bar g_{\mu\nu}$. Its time-time and time-space components yield the [scalar gauge transformations with a background lapse](../../../../../../scalar-gauge-transformations-with-a-background-lapse.md):

$$
\widetilde\Psi=\Psi-\dot\xi^0-\frac{\dot{\bar N}}{\bar N}\xi^0,\qquad \widetilde B=B+\frac{\bar N^2}{a^2}\xi^0-\dot\lambda.
$$

For example, $\bar g_{00}=-\bar N^2$ gives $-(\mathcal L_\xi\bar g)_{00}=2\bar N\dot{\bar N}\xi^0+2\bar N^2\dot\xi^0$; $\bar g_{0i}=0$ gives $-(\mathcal L_\xi\bar g)_{0i}=\bar N^2\partial_i\xi^0-a^2\partial_i\dot\lambda$. These establish the signs directly.

To preserve [synchronous gauge in cosmology](../../../../../../synchronous-gauge-in-cosmology.md), both transformed quantities must remain zero. Hence

$$
\partial_t(\bar N\xi^0)=0,\qquad\dot\lambda=\frac{\bar N^2}{a^2}\xi^0.
$$

Integrating gives the [residual synchronous-gauge freedom](../../../../../../residual-synchronous-gauge-freedom.md)

$$
\boxed{\xi^0=\frac{C(\mathbf x)}{\bar N(t)},\qquad\lambda=C(\mathbf x)\int^t\frac{\bar N(t')}{a(t')^2}\,dt'+D(\mathbf x).}
$$

The integration lower limit can be absorbed into $D$. Spatially homogeneous additions to $\lambda$ generate no spatial displacement, so they are physically irrelevant to this scalar parametrization.

The spatial transformation also gives $\widetilde\Phi=\Phi+(\dot a/a)\xi^0$ and $\widetilde E=E+\lambda$. Thus fixing the lapse and shift perturbations does not fix the entire coordinate system; the arbitrary functions $C,D$ can still change the remaining [scalar cosmological perturbations](../../../../../../scalar-cosmological-perturbation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
