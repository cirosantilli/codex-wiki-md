<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\gamma:[0,\ell]\to M$ be a unit-speed [geodesic](../../../../../../geodesic.md), let $F(s,t)$ be a smooth variation with fixed endpoints, and let

$$
T=\dot\gamma,
\qquad
V=\left.\frac{\partial F}{\partial s}\right|_{s=0}
$$

be its [variation vector field](../../../../../../variation-vector-field.md). Then $V(0)=V(\ell)=0$. If $V^\perp=V-\langle V,T\rangle T$ is its component normal to $\gamma$, the [second variation of Riemannian arc length](../../../../../../second-variation-of-riemannian-arc-length.md) is

$$
\left.\frac{d^2}{ds^2}L(F(s,\cdot))\right|_{s=0}
=I(V^\perp,V^\perp)
=\int_0^\ell\left(
|D_tV^\perp|^2-
\langle R(V^\perp,T)T,V^\perp\rangle
\right)dt.
$$

Here $D_t=\nabla_T$ is the [covariant derivative](../../../../../../covariant-derivative.md) along $\gamma$, $R$ is the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md), and $I$ is the [Riemannian index form](../../../../../../riemannian-index-form.md). Fixed endpoints remove the boundary term. The normal projection removes a tangential change of parametrization, which does not change length to second order.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 131](../../../paper-131-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
