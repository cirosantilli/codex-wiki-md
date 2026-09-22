<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Preserving [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md) means keeping both $\delta g_{00}$ and $\delta g_{0i}$ zero. Applying the metric transformation to the background gives

$$
\delta\widetilde g_{00}=2a^2[(\xi^0)'+\mathcal H\xi^0],\qquad
\delta\widetilde g_{0i}=a^2[\partial_i\xi^0-(\xi^i)'].
$$

The first equation requires $(a\xi^0)'=0$, so $\xi^0=C(\mathbf x)/a$. For the scalar displacement $\xi^i=\partial^i\lambda$, the second requires $\lambda'=\xi^0$, up to a spatially homogeneous coordinate displacement that does not affect scalar perturbations. Integrating gives

$$
\boxed{\xi^0=\frac{C(\mathbf x)}a,\qquad\lambda=C(\mathbf x)\int^\tau\frac{d\tau'}{a(\tau')}+D(\mathbf x).}
$$

This is the [residual gauge freedom in synchronous gauge](../../../../../../residual-synchronous-gauge-freedom.md). The lapse and shift conditions do not uniquely choose a slicing and spatial labeling.

A background density is a scalar, so under this remaining time displacement

$$
\widetilde\delta=\delta-\frac{\bar\rho'}{\bar\rho}\xi^0.
$$

For a fluid with constant equation of state, background conservation gives $\bar\rho'/\bar\rho=-3(1+w)\mathcal H$, hence

$$
\boxed{\Delta\delta=3(1+w)\frac{\mathcal HC(\mathbf x)}a.}
$$

The [synchronous density gauge mode](../../../../../../synchronous-density-gauge-mode.md) scales as $\tau^{-2}$ in [radiation domination](../../../../../../radiation-domination.md) and as $\tau^{-3}$ in [matter domination](../../../../../../matter-domination.md). It can mimic a changing density perturbation without changing physical observables. A density time dependence alone therefore does not identify a physical growing or decaying mode. Choosing coordinates comoving with cold matter fixes the residual time freedom, and a remaining spatial relabeling fixes the initial metric-trace integration convention. Gauge-invariant curvature perturbations provide another way to specify physical initial conditions.

For consistency, linear metric theory requires all background-orthonormal components of $h_{ij}$ to be small. The PDF's small-determinant condition by itself is insufficient: $h_{ij}=\operatorname{diag}(L,0,0)$ has zero determinant even for large $L$. This is [small determinant does not imply a small metric perturbation](../../../../../../small-determinant-does-not-imply-a-small-metric-perturbation.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
