<h1 id="37d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
L(x,\dot x)=\sqrt{g_{\mu\nu}\dot x^\mu\dot x^\nu}
=\frac{ds}{d\lambda}.
$$

The [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) gives

$$
\frac d{d\lambda}\left(\frac{g_{\beta\nu}\dot x^\nu}{L}\right)
-\frac1{2L}\partial_\beta g_{\mu\nu}
\dot x^\mu\dot x^\nu=0.
$$

Since $\dot x^\mu=L\,dx^\mu/ds$ and $d/d\lambda=L\,d/ds$, this becomes

$$
\frac d{ds}\left(g_{\beta\nu}\frac{dx^\nu}{ds}\right)
-\frac12\partial_\beta g_{\mu\nu}
\frac{dx^\mu}{ds}\frac{dx^\nu}{ds}=0.
$$

Expanding the derivative, multiplying by the inverse metric, and using the [Christoffel symbol](../../../../../../christoffel-symbol.md)

$$
\Gamma^\alpha_{\mu\nu}
=\frac12g^{\alpha\beta}
(\partial_\mu g_{\beta\nu}
+\partial_\nu g_{\beta\mu}
-\partial_\beta g_{\mu\nu})
$$

gives the [geodesic equation](../../../../../../geodesic-equation.md)

$$
\boxed{
\frac{d^2x^\alpha}{ds^2}
+\Gamma^\alpha_{\mu\nu}
\frac{dx^\mu}{ds}\frac{dx^\nu}{ds}=0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [37D](../../37d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
