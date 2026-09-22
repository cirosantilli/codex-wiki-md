<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Parametrize the data by $(\xi,\eta,\zeta)=(\cos\theta,\sin\theta,-1)$. The determinant testing [Noncharacteristic Cauchy data](../../../../../noncharacteristic-cauchy-data.md) is

$$
\det\begin{pmatrix}-\sin\theta&\cos\theta\sin\theta\\
\cos\theta&\sin^2\theta\end{pmatrix}=-\sin\theta.
$$

Thus the open upper and lower semicircles are noncharacteristic, but the entire circle is not a valid noncharacteristic data curve: the determinant vanishes at $(1,0)$ and $(-1,0)$.

There is a stronger obstruction at those two points. On $y=0$, the differential equation forces $0=-z^4/3$, and hence $z=0$. This contradicts the prescribed value $z=-1$ at both endpoints. Therefore

$$
\boxed{\text{No classical solution satisfies the data on the entire circle.}}
$$

The obstruction is already present if the equation is imposed next to the circle and the solution and its first [partial derivatives](../../../../../partial-derivative.md) extend continuously to it.

Away from the endpoints, the [characteristic projections](../../../../../characteristic-projection.md) are radial half-lines:

$$
(x,y)=r(\cos\theta,\sin\theta),\qquad r=\frac1{1-s\sin\theta}>0.
$$

For $\sin\theta>0$, $r$ increases with $s$; for $\sin\theta<0$, $r$ decreases with $s$. Each projection meets its own open semicircle exactly once and never crosses $y=0$. The endpoint projections themselves are single stationary points, although their lifted [characteristic curves](../../../../../characteristic-curve.md) have varying height.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
