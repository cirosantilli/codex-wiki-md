<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

For fixed endpoints, the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\boxed{\frac{d}{dx}f_{y'}-f_y=0.}
$$

Let the sphere have radius $R$ and write the speed as $v_0\sin\theta$, with $v_0>0$. The infinitesimal travel time in the interior $0<\theta<\pi$ is

$$
dt=\frac R{v_0}\sqrt{\frac{d\theta^2}{\sin^2\theta}+d\phi^2}.
$$

This is the [flat-cylinder travel metric for sine-latitude speed](../../../../../flat-cylinder-travel-metric-for-sine-latitude-speed.md). Introduce

$$
z=\operatorname{arsinh}(\cot\theta),\qquad dz=-\frac{d\theta}{\sin\theta}.
$$

The travel-time metric becomes $(R/v_0)\sqrt{dz^2+d\phi^2}$, an ordinary Euclidean metric on a cylinder because $\phi$ is periodic. After choosing a lift of $\phi$, shortest paths are straight segments in $(\phi,z)$. For a route that is a graph over $\phi$, the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) for $\sqrt{1+(dz/d\phi)^2}$ reads

$$
\frac{d}{d\phi}\left(\frac{z'}{\sqrt{1+z'^2}}\right)=0.
$$

Thus $z'=A$ is constant and $z=A\phi+B$. Transforming back,

$$
\boxed{\sinh(A\phi+B)=\cot\theta.}
$$

This proves the requested form for nonmeridional routes, including the equator when $A=B=0$. It is also globally minimizing for its chosen azimuthal lift: Euclidean arc length is at least the straight-line separation, and the shortest lift minimizes that separation among angular differences differing by $2\pi$.

There is a coordinate exception to the printed universal form. When the shortest angular separation is zero, the fastest path is the meridian $\phi=\text{constant}$; it is a vertical straight line on the cylinder and cannot be represented by finite $A,B$ as a graph over $\phi$. The poles correspond to $z=\pm\infty$ and cannot be reached in finite time with this speed law.

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
