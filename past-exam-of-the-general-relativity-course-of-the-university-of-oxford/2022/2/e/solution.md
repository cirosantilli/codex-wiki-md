<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In standard [spherical coordinates](../../../../spherical-coordinate-system.md), parametrize the [two-sphere](../../../../two-sphere.md) by

$$
\mathbf x(\theta,\phi)=R(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta).
$$

The [coordinate basis](../../../../coordinate-basis.md) transforms from the fixed Cartesian basis according to $\mathbf e_a=(\partial x^i/\partial q^a)\mathbf e_i$. Therefore

$$
\begin{aligned}
\mathbf e_\theta&=\partial_\theta\mathbf x
=R(\cos\theta\cos\phi,\cos\theta\sin\phi,-\sin\theta),\\
\mathbf e_\phi&=\partial_\phi\mathbf x
=R(-\sin\theta\sin\phi,\sin\theta\cos\phi,0).
\end{aligned}
$$

Their [inner products](../../../../inner-product-split.md) are $\mathbf e_\theta^2=R^2$, $\mathbf e_\theta\cdot\mathbf e_\phi=0$ and $\mathbf e_\phi^2=R^2\sin^2\theta$. Thus the [induced metric](../../../../induced-metric.md) is

$$
\boxed{(g_{ij})=R^2\begin{pmatrix}1&0\\0&\sin^2\theta\end{pmatrix},\qquad
ds^2=R^2(d\theta^2+\sin^2\theta\,d\phi^2).}
$$

The source's intermediate display places an extra $R^2$ outside entries already labelled $g_{\theta\theta},\ldots$. Interpreting those entries as the actual [metric tensor](../../../../metric-tensor.md) components would double-count the factor: for example, $R=2$ gives $g_{\theta\theta}=4$ directly from $\mathbf e_\theta^2$, not $16$. Its final matrix is the correct [induced metric](../../../../induced-metric.md); the entries of its intermediate matrix must instead denote dimensionless coefficients.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
