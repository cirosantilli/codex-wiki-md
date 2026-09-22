<h1 id="35e/solution">Solution</h1>

↑ **Parent:** [35E](../35e.md)

An affinely parametrized [geodesic](../../../../../geodesic.md) satisfies $d^2x^a/d\lambda^2+\Gamma^a{}_{bc}T^bT^c=0$, which is exactly $\nabla_TT=0$. The [Levi-Civita connection](../../../../../levi-civita-connection.md) is metric-compatible, so

$$
\frac d{d\lambda}g(X,Y)=(\nabla_Tg)(X,Y)+g(\nabla_TX,Y)+g(X,\nabla_TY)=0
$$

when both vectors are parallel transported. **Their inner product is constant**, including their lengths; this preservation in fact holds along any path with parallel vectors, not only a [geodesic](../../../../../geodesic.md).

For the two-parameter family, mixed partial derivatives commute and $\Gamma^a{}_{bc}$ is symmetric in its lower indices. Consequently

$$
\nabla_TS^a=\partial_\lambda\partial_\mu x^a+\Gamma^a{}_{bc}S^bT^c=\nabla_ST^a.
$$

Using this equality and the supplied [curvature](../../../../../curvature.md)-commutator convention,

$$
\nabla_T^2S=\nabla_T\nabla_ST=\nabla_S\nabla_TT+[\nabla_T,\nabla_S]T=R(T,S)T.
$$

In components the [geodesic deviation](../../../../../geodesic-deviation.md) equation is

$$
\boxed{\nabla_T^2S^a=R^a{}_{bcd}T^bT^cS^d.}
$$

It describes the relative acceleration of nearby freely falling worldlines. A freely falling observer can remove the connection at an event by choosing a local inertial frame, but cannot remove the [curvature](../../../../../curvature.md)-dependent tidal acceleration of neighboring freely falling particles. Measuring their separation and relative acceleration therefore measures the local gravitational tidal field.

## ↑ Ancestors (10)

1. [35E](../35e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
