<h1 id="25i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [first fundamental form](../../../../../../first-fundamental-form.md) of an embedded surface $S\subseteq\mathbb R^3$ is the inner product induced on each tangent plane:

$$
I_p(u,v)=u\cdot v,
\qquad u,v\in T_pS.
$$

For a tangent vector field $V$ along a curve $\alpha$, its [surface covariant derivative](../../../../../../surface-covariant-derivative.md) is

$$
\frac{DV}{dt}=\left(\frac{dV}{dt}\right)^\top,
$$

the tangential projection of its ordinary derivative. A curve is a [geodesic](../../../../../../geodesic.md) when

$$
\frac{D\dot\alpha}{dt}=0.
$$

A [local isometry](../../../../../../local-isometry.md) preserves the first fundamental form, so its Christoffel symbols and Levi--Civita covariant derivatives satisfy

$$
\nabla^R_{(\phi\circ\alpha)'}(D\phi V)
=D\phi(\nabla^S_{\alpha'}V).
$$

Taking $V=\alpha'$ shows that if $\alpha$ is geodesic, then $\phi\circ\alpha$ is geodesic.

The converse is false. The dilation

$$
\phi:\mathbb R^2\to\mathbb R^2,
\qquad \phi(x)=2x,
$$

maps every affinely parametrized straight-line geodesic to another such geodesic, but

$$
|D\phi(v)|=2|v|,
$$

so it does not preserve the first fundamental form. This is the [geodesic-preserving homothety that is not a local isometry](../../../../../../geodesic-preserving-homothety-that-is-not-a-local-isometry.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25I](../../25i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
