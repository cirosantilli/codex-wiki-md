<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For $0<b-a<2\pi$, let $D=\mathbf r([a,b]\times[c,d])$ and use the [orientation of a surface](../../../../orientation-of-a-surface.md) determined by $N=\mathbf r_u\times\mathbf r_v/|\mathbf r_u\times\mathbf r_v|$. Its positive [boundary orientation](../../../../boundary-orientation.md) follows the bottom side in increasing $u$, the right side in increasing $v$, the top side in decreasing $u$, and the left side in decreasing $v$. The [Gauss-Bonnet theorem](../../../../gauss-bonnet-theorem.md) for this disc with four corners reads

$$
\int_D\kappa\,dA+\int_{\partial D}\kappa_g\,ds+\sum_{j=1}^4\varepsilon_j=2\pi,
$$

where the $\varepsilon_j$ are the signed exterior [angles](../../../../angle.md).

The bottom and top sides have cancelling [geodesic curvature](../../../../geodesic-curvature.md) integrals: a [screw motion](../../../../screw-motion.md) takes one to the other with opposite [boundary orientation](../../../../boundary-orientation.md). Explicitly, along increasing $u$ at fixed $v$, the [speed](../../../../speed.md) is one and the signed [geodesic curvature](../../../../geodesic-curvature.md) is $-\sin u/\sqrt{1+\sin^2u}$ on both sides. The right and left sides contribute, respectively, the integral along $\gamma_b$ and minus the integral along $\gamma_a$.

Although the coordinate sides are generally not perpendicular, the corner contributions still sum to $2\pi$. Indeed, let $\theta(u)$ be the [angle](../../../../angle.md) between $\mathbf r_u$ and $\mathbf r_v$, so

$$
\cos\theta(u)=\frac{1+\cos u}{\sqrt{3+2\cos u}}.
$$

Starting at the bottom-left corner, the exterior [angles](../../../../angle.md) are $\pi-\theta(a)$, $\theta(b)$, $\pi-\theta(b)$ and $\theta(a)$. Their sum is $2\pi$. Cancelling this from the [Gauss-Bonnet theorem](../../../../gauss-bonnet-theorem.md) leaves

$$
\int_D\kappa\,dA=\int_{\gamma_a}\kappa_g\,ds-\int_{\gamma_b}\kappa_g\,ds,
$$

which is the identity in part (e). For a rectangle covering more than one turn, apply the same argument on the parameter rectangle with its induced [Riemannian metric](../../../../riemannian-metric-split.md), or partition it into narrower rectangles and cancel the artificial internal [boundary](../../../../boundary-of-a-set.md) contributions. This gives the version counting multiplicity, as required by the correction in part (e).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the geometry of surfaces course of the University of Oxford](../../../split.md)
5. [Geometry of surfaces course of the University of Oxford](../../../../geometry-of-surfaces-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
