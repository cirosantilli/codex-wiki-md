<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Parametrize the nonconstant [closed geodesic](../../../../../../closed-geodesic.md) at unit speed on $[0,L]$. Its [parallel transport](../../../../../../parallel-transport.md) around the loop fixes the tangent $\dot\gamma(0)$. Since the manifold is orientable, it preserves orientation on the full [tangent space](../../../../../../tangent-space.md), and hence has determinant one on the normal space. This normal space has odd dimension because the manifold has even dimension.

An [odd-dimensional special orthogonal transformation has a fixed vector](../../../../../../odd-dimensional-special-orthogonal-transformation-has-a-fixed-vector.md). Indeed, nonreal [eigenvalues](../../../../../../eigenvalue.md) of a real orthogonal transformation occur in conjugate pairs with product one; the real [eigenvalues](../../../../../../eigenvalue.md) are $\pm1$, and determinant one makes the number of $-1$ [eigenvalues](../../../../../../eigenvalue.md) even. Odd dimension therefore requires a $+1$ [eigenvalue](../../../../../../eigenvalue.md). Transport a unit fixed normal vector around the [geodesic](../../../../../../geodesic.md) to obtain a periodic parallel field $V$, with $D_tV=0$ and $V\perp\dot\gamma$.

The variation $\gamma_s(t)=\exp_{\gamma(t)}(sV(t))$ is defined uniformly for small $s$, because the image of the original loop is [compact](../../../../../../compact-space.md). Periodicity gives closed curves and a [homotopy](../../../../../../homotopy.md) through loops. With the standard positive-sectional-curvature [Riemannian index form](../../../../../../riemannian-index-form.md), the [second variation of geodesic energy](../../../../../../second-variation-of-geodesic-energy.md) is

$$
E''(0)=I(V,V)=\int_0^L\bigl(|D_tV|^2-K(\dot\gamma,V)\bigr)dt
=-\int_0^LK(\dot\gamma,V)\,dt<0.
$$

The first variation vanishes for a [closed geodesic](../../../../../../closed-geodesic.md), since the endpoint terms cancel. Therefore $E(\gamma_s)<E(\gamma_0)=L/2$ for sufficiently small nonzero $s$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\operatorname{length}(\gamma_s)^2\leq L\int_0^L|\dot\gamma_s|^2dt
=2LE(\gamma_s)<L^2.
$$

Thus **the [closed geodesic](../../../../../../closed-geodesic.md) is homotopic to a strictly shorter closed curve**. This proves the [instability of a closed geodesic in positive even-dimensional curvature](../../../../../../instability-of-a-closed-geodesic-in-positive-even-dimensional-curvature.md); completeness of the manifold is unnecessary for this compact-loop variation. Constant loops are excluded by the usual nonconstant meaning of a [closed geodesic](../../../../../../closed-geodesic.md) in this assertion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
