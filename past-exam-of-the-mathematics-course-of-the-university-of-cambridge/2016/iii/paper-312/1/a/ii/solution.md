<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $h=\det h_{ij}$. Contract the [extrinsic curvature with a negative shift](../../../../../../../extrinsic-curvature-with-a-negative-shift.md) with $h^{ij}$. The [Jacobi determinant derivative formula](../../../../../../../jacobi-determinant-derivative-formula.md) and metric compatibility give

$$
h^{ij}\dot h_{ij}=\partial_t\ln h=\frac{\dot h}{h},\qquad h^{ij}D_iN_j=D_iN^i.
$$

Consequently

$$
\boxed{K=-\frac{1}{2N}\left(\frac{\dot h}{h}+2D_iN^i\right).}
$$

The local volume element is $\sqrt h\,d^3x$, so for zero [shift vector](../../../../../../../shift-vector.md) the proper-time derivative along the normal is $d/ds=N^{-1}\partial_t$ and

$$
\theta=\frac1N\partial_t\ln\sqrt h=-K.
$$

Here $\theta$ is the [expansion scalar](../../../../../../../expansion-scalar.md). Writing $a_{\mathrm{loc}}=h^{1/6}$ defines a local linear scale from this volume, whence the [local volume Hubble parameter](../../../../../../../local-volume-hubble-parameter.md) is

$$
\boxed{H_{\mathrm{loc}}=\frac{1}{a_{\mathrm{loc}}}\frac{da_{\mathrm{loc}}}{ds}=\frac{\dot a_{\mathrm{loc}}}{Na_{\mathrm{loc}}}=-\frac K3.}
$$

The factor of three converts volume expansion into linear expansion, and $N$ converts coordinate time into proper time. This agrees with the usual [Hubble parameter](../../../../../../../hubble-parameter.md) in a homogeneous [FLRW metric](../../../../../../../friedmann-lemaitre-robertson-walker-metric.md).

For a volume-shape decomposition the [unimodular spatial metric](../../../../../../../unimodular-spatial-metric.md) is $\gamma_{ij}=a_{\mathrm{loc}}^{-2}h_{ij}$, with determinant one. If instead the printed positive power $a_{\mathrm{loc}}^2h_{ij}$ is taken literally, its determinant is $a_{\mathrm{loc}}^{12}$; it is a conformal rescaling but not the unimodular shape metric. The trace calculation does not need that rescaling.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
