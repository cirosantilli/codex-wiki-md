<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use spatial indices $i,j=1,2,3$, set $\phi_i=\partial_i\phi$, and assume $\phi$ is smooth. The [inverse metric](../../../../../../inverse-metric.md) has $g^{tt}=-c^{-2}e^{-2\phi/c^2}$ and $g^{ij}=\delta^{ij}$. The [Christoffel symbols](../../../../../../christoffel-symbol.md) of the [Levi-Civita connection](../../../../../../levi-civita-connection.md) follow from $\Gamma^\alpha{}_{\beta\gamma}=g^{\alpha\delta}(\partial_\beta g_{\gamma\delta}+\partial_\gamma g_{\beta\delta}-\partial_\delta g_{\beta\gamma})/2$:

$$
\boxed{\Gamma^t{}_{ti}=\Gamma^t{}_{it}=\frac{\phi_i}{c^2},\qquad \Gamma^i{}_{tt}=e^{2\phi/c^2}\phi_i.}
$$

All other components vanish. Although $g_{tt}=-c^2-2\phi+O(c^{-2})$ diverges, its [affine connection](../../../../../../affine-connection.md) has a smooth limit on compact subsets:

$$
\boxed{\Gamma^{(\infty)i}{}_{tt}=\phi_i,\qquad \text{all other limiting components}=0.}
$$

This is the [Newtonian connection from an exponential lapse](../../../../../../newtonian-connection-from-an-exponential-lapse.md). It is [torsion-free](../../../../../../torsion-free-connection.md), and its [geodesic equation](../../../../../../geodesic-equation.md), using $t$ as an [affine parameter](../../../../../../affine-parameter.md) when $\dot t\ne0$, is $d^2x^i/dt^2=-\partial_i\phi$. Thus $\phi$ has the role of a [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md). There is no finite limiting nondegenerate [Lorentzian metric](../../../../../../lorentzian-metric.md) in these fixed coordinates; $-g(c)/c^2$ tends to $dt^2$, a rank-one tensor. The limiting connection preserves $dt$ and the contravariant spatial tensor with components $h^{ij}=\delta^{ij}$, $h^{t\mu}=0$, which describe the degenerate temporal/spatial structures of this limit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
