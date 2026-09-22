<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\gamma_{ij}$ denote the spatial [induced metric](../../../../../../induced-metric.md) and $\gamma=\det\gamma_{ij}$. Its conformally rescaled version $\widetilde\gamma_{ij}=\gamma^{-1/3}\gamma_{ij}$ has determinant one. The [Jacobi determinant derivative formula](../../../../../../jacobi-determinant-derivative-formula.md) consequently gives

$$
\gamma^{ij}\dot\gamma_{ij}=\frac{\dot\gamma}{\gamma},
\qquad \widetilde\gamma^{ij}\dot{\widetilde\gamma}_{ij}=0.
$$

Thus the determinant measures the volume-changing part of the spatial metric, while the unit-determinant part contains shape changes. [Metric compatibility](../../../../../../metric-compatibility.md) for the spatial [covariant derivative](../../../../../../covariant-derivative.md) also gives $\gamma^{ij}D_iN_j=D_iN^i$.

There is a sign inconsistency in the PDF. Contracting its defining expression for $K_{ij}$, with its threading convention $dx^i-N^idt$ and its future normal $n^\mu=N^{-1}(1,N^i)$, gives

$$
\boxed{K=-\frac1{2N}\left(\frac{\dot\gamma}{\gamma}+2D_iN^i\right),}
$$

not the displayed trace with a minus sign before the divergence. This is the [trace of extrinsic curvature with a negative shift](../../../../../../trace-of-extrinsic-curvature-with-a-negative-shift.md). For a concrete check, take $\gamma_{ij}=\delta_{ij}$, $N=1$ and $N^i=bx^i$. The defining formula gives $K_{ij}=-b\delta_{ij}$ and $K=-3b$, whereas the printed trace would give $+3b$. Reversing the shift convention can produce the other trace formula, but also changes the shift terms in $K_{ij}$ and the normal; the two conventions cannot be combined.

For the requested expansion interpretation, set the [shift vector](../../../../../../shift-vector.md) to zero. The sign discrepancy then disappears. A small coordinate volume has proper volume proportional to $\sqrt\gamma$, and proper time along its normal is $ds=Ndt$. Its expansion rate is

$$
\theta=\frac1N\partial_t\log\sqrt\gamma=-K.
$$

Therefore

$$
\boxed{H_{\rm local}=-\frac K3=\frac1{3N}\partial_t\log\sqrt\gamma
=\frac1N\partial_t\log(\gamma^{1/6}).}
$$

This is the [local volume Hubble parameter](../../../../../../local-volume-hubble-parameter.md), the mean of the three local directional expansion rates. In a homogeneous isotropic background $\gamma=a^6$, it reduces to $\dot a/(Na)$. The interpretation does not require the local expansion to be isotropic: the trace-free part of the [extrinsic curvature](../../../../../../extrinsic-curvature.md) can still describe shear.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
