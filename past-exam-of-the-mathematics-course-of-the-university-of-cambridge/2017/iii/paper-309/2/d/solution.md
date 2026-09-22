<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use $x^0=t$ and the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) $\epsilon^1{}_{23}=1$. Define a smooth [affine connection](../../../../../../affine-connection.md) by

$$
\boxed{\Gamma^i{}_{00}=-E^i,\qquad \Gamma^i{}_{0j}=\Gamma^i{}_{j0}=\epsilon^i{}_{jk}B^k,\qquad \Gamma^0{}_{ab}=\Gamma^i{}_{jk}=0.}
$$

The lower indices are symmetric, so it is a [torsion-free connection](../../../../../../torsion-free-connection.md). With $t$ itself as parameter, the time component of the [geodesic equation](../../../../../../geodesic-equation.md) is identically satisfied, while its spatial components become

$$
\ddot x^i=-\Gamma^i{}_{00}-2\Gamma^i{}_{0j}\dot x^j=E^i+2\epsilon^i{}_{kj}B^k\dot x^j.
$$

The last term is $2(\mathbf B\times\dot{\mathbf x})^i$, with the wedge in the source interpreted as the three-dimensional [cross product](../../../../../../cross-product.md). Thus the spacetime lifts $(t,\mathbf x(t))$ are actually affinely parametrized [geodesics](../../../../../../geodesic.md), which proves the requested unparametrized claim. Conversely a geodesic with nonzero constant $dt/ds$ can be parametrized by $t$ and obeys this particle equation; purely spatial geodesics with $dt/ds=0$ are not such trajectories. No field equations or metric compatibility are needed. This construction is the [affine connection for a velocity-linear force](../../../../../../affine-connection-for-a-velocity-linear-force.md).

## ↑ Ancestors (11)

1. [D](../d.md)
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
