<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

Write the cone as $z=r\cot\alpha$, with $r$ the distance from its axis and $0<\alpha<\pi/2$. Its [Euclidean metric](../../../../../euclidean-metric.md) gives

$$
ds^2=dr^2+r^2d\theta^2+dz^2=\csc^2\alpha\,dr^2+r^2d\theta^2.
$$

Consequently a differentiable path expressed as $r=r(\theta)$ has [arc length](../../../../../arc-length.md)

$$
\boxed{S=\int\sqrt{r^2+\csc^2\alpha\,(r')^2}\,d\theta.}
$$

For $L(r,r')=\sqrt{r^2+\csc^2\alpha(r')^2}$, the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) has the [Beltrami identity](../../../../../beltrami-identity.md) because $L$ has no explicit $\theta$ dependence:

$$
L-r'\frac{\partial L}{\partial r'}=\frac{r^2}{L}=C.
$$

For a nonradial minimizing path, $C>0$. Rearranging and integrating gives

$$
(r')^2=\sin^2\alpha\,r^2\left(\frac{r^2}{C^2}-1\right),\qquad \boxed{r\cos\bigl((\theta-\theta_0)\sin\alpha\bigr)=C.}
$$

The endpoint conditions determine $C$ and $\theta_0$ on the selected angular branch.

To verify that this stationary path really minimizes [arc length](../../../../../arc-length.md), use the [local isometry from a circular cone to the plane](../../../../../local-isometry-from-a-circular-cone-to-the-plane.md). Set $s=r/\sin\alpha$ and $\phi=\theta\sin\alpha$; then $ds^2+s^2d\phi^2$ is the plane [metric](../../../../../metric.md). The displayed path is a straight line $s\cos(\phi-\phi_0)=C/\sin\alpha$, so its segment realizes the plane distance. Choose endpoint angular lifts with $|\Delta\theta|\leq\pi$; then $|\Delta\phi|<\pi$, and the joining segment avoids the apex. Its length is

$$
\frac1{\sin\alpha}\sqrt{r_1^2+r_2^2-2r_1r_2\cos(\sin\alpha\,\Delta\theta)}.
$$

Other lifts with developed angular difference less than $\pi$ give at least this distance; an angular change of at least $\pi$ has infimum at least $s_1+s_2$, attained only if passage through the apex is allowed. This proves the global choice above. Endpoints on a common generator have the radial segment as shortest path, which is the limiting case omitted by the $r(\theta)$ parametrization. If an endpoint is the apex, its shortest path is a generator. Thus **shortest paths are straight segments after developing the cone**.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
