<h1 id="12a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [spherical circle](../../../../../../spherical-circle.md), use a [rotation](../../../../../../rotation-mathematics.md) to put the center at the north pole. Points at [spherical distance](../../../../../../great-circle-distance.md) $r$ have polar angle $r$ and admit the parametrization

$$
\gamma(\theta)=(\sin r\cos\theta,\sin r\sin\theta,\cos r),\qquad0\le\theta\le2\pi.
$$

Its speed is $|\gamma'(\theta)|=\sin r$, so the [arc length](../../../../../../arc-length.md) is

$$
\boxed{C(r)=2\pi\sin r.}
$$

For small $r$, the [Taylor series](../../../../../../taylor-series.md) gives $C(r)=2\pi r-(\pi/3)r^3+O(r^5)$. Thus its circumference is smaller than the Euclidean circumference $2\pi r$ for the same intrinsic radius. Their ratio is $\sin r/r=1-r^2/6+O(r^4)$ and tends to one. The leading agreement expresses local Euclidean behavior; the cubic deficit reflects the positive [Gaussian curvature](../../../../../../gaussian-curvature.md) of the unit sphere.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12A](../../12a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
