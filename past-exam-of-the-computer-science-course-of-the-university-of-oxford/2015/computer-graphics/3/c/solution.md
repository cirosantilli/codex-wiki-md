<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the oriented vertices be $a,b,c$, in an order such that $n=(b-a)\times(c-a)$ points out of the front face. The given nondegeneracy guarantees $n\ne0$. A [ray](../../../../../ray-geometry.md) with nonzero direction $r$ approaches the front face only if

$$
n\cdot r<0.
$$

Reject $n\cdot r\geq0$. This combines [back-face culling](../../../../../back-face-culling.md) with rejection of parallel rays, including the coplanar case for this ordinary surface-hit test. The [ray-plane intersection](../../../../../ray-plane-intersection.md) parameter is

$$
\lambda=\frac{n\cdot(a-o)}{n\cdot r}.
$$

Reject $\lambda<0$; for rays launched from existing surfaces use a positive lower cutoff to avoid counting the launch surface. Form $p=o+\lambda r$.

Finally determine whether $p$ lies inside the [triangle](../../../../../triangle.md). For $u=b-a$, $v=c-a$, $w=p-a$, compute

$$
D=(u\cdot u)(v\cdot v)-(u\cdot v)^2>0,
$$



$$
\beta=\frac{(v\cdot v)(w\cdot u)-(u\cdot v)(w\cdot v)}D,\qquad
\gamma=\frac{(u\cdot u)(w\cdot v)-(u\cdot v)(w\cdot u)}D.
$$

These solve $p=a+\beta u+\gamma v$. The [barycentric coordinates](../../../../../barycentric-coordinate-system.md) are $(1-\beta-\gamma,\beta,\gamma)$, so the complete acceptance criterion is

$$
\boxed{n\cdot r<0,\quad \lambda\geq0,\quad\beta\geq0,\quad\gamma\geq0,\quad\beta+\gamma\leq1;\qquad p=o+\lambda r.}
$$

The inequalities include the edges and vertices. A renderer sharing edges between [triangles](../../../../../triangle.md) should use a consistent numerical edge convention; small [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md) errors near a shared boundary should not create cracks. Normalizing $n$ is unnecessary for this intersection calculation because its scale cancels.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Computer graphics](../../../computer-graphics-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
