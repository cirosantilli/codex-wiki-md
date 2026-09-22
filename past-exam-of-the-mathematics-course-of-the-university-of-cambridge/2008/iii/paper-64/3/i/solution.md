<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\gamma_{ij}={}^{(3)}g_{ij}$, $\gamma=\det\gamma_{ij}$ and $D_i$ for the [spatial covariant derivative](../../../../../../spatial-covariant-derivative.md). With the negative-shift convention, the [extrinsic curvature of a spatial hypersurface](../../../../../../extrinsic-curvature-of-a-spatial-hypersurface.md) is $K_{ij}=-(\dot\gamma_{ij}+D_iN_j+D_jN_i)/(2N)$. Contracting with $\gamma^{ij}$ and using metric compatibility gives

$$
K=-\frac1{2N}\left(\gamma^{ij}\dot\gamma_{ij}+2D_iN^i\right).
$$

The logarithmic [determinant](../../../../../../determinant.md) identity makes $\gamma^{ij}\dot\gamma_{ij}=\dot\gamma/\gamma$, hence

$$
\boxed{K=-\frac1{2N}\left(\frac{\dot\gamma}{\gamma}+2D_iN^i\right).}
$$

This is also the fractional volume expansion, with a minus sign from the extrinsic-curvature convention.

Define $a=\gamma^{1/6}$ so that $\sqrt\gamma=a^3$. The useful unit-determinant conformal decomposition is $\gamma_{ij}=a^2\widetilde\gamma_{ij}$ with $\det\widetilde\gamma=1$, equivalently $\widetilde\gamma_{ij}=a^{-2}\gamma_{ij}$. Multiplying by $a^2$ instead would be a different conformal rescaling, not this unit-determinant one; no conformal decomposition is needed for the trace identity itself.

With zero [shift vector](../../../../../../shift-vector.md), $\dot\gamma/\gamma=6\dot a/a$ and the [local volume Hubble parameter](../../../../../../local-volume-hubble-parameter.md) is

$$
\boxed{H=-\frac K3=\frac1{Na}\dot a.}
$$

Along a normal trajectory proper time satisfies $ds=Ndt$, so $H=a^{-1}da/ds$ is the local physical volume-expansion rate. The printed equality with $\dot a/a$ requires the proper-time gauge $N=1$; zero shift alone does not set the lapse to unity. In a homogeneous [Friedmann-Lemaître-Robertson-Walker metric](../../../../../../friedmann-lemaitre-robertson-walker-metric.md) it reduces to the ordinary [Hubble parameter](../../../../../../hubble-parameter.md), while in an inhomogeneous spacetime it can vary from one normal trajectory to another.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
