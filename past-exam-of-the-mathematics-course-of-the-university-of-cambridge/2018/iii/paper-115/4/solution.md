<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [energy of a curve](../../../../../energy-of-a-curve.md) normalization

$$
E(\gamma)=\frac12\int_a^b|\dot\gamma|_g^2\,dt.
$$

For a variation $F(s,t)$ put $T=\partial_tF$ and $V=\partial_sF$. The [Levi-Civita connection](../../../../../levi-civita-connection.md) is torsion free, so $\nabla_sT=\nabla_tV$. Differentiating energy once gives $E'=[\langle V,T\rangle]_a^b-\int\langle V,\nabla_tT\rangle$. Along a geodesic, $\nabla_tT=0$. Differentiating again, commuting covariant derivatives, and integrating by parts gives the [second variation of geodesic energy](../../../../../second-variation-of-geodesic-energy.md):

$$
\boxed{E''(0)=
[\langle\nabla_sV,T\rangle]_a^b+
\int_a^b\bigl(|\nabla_tV|^2-\langle R(V,T)T,V\rangle\bigr)\,dt.}
$$

The curvature convention is $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$, consistent with the specified positive [sectional curvature](../../../../../sectional-curvature.md). Indeed $\nabla_s\nabla_tV=\nabla_t\nabla_sV+R(V,T)V$, and $\langle R(V,T)V,T\rangle=-\langle R(V,T)T,V\rangle$. The endpoint term vanishes for fixed endpoints or for periodic variations of a closed geodesic. The integral is the [Riemannian index form](../../../../../riemannian-index-form.md) $I(V,V)$.

Let $\dim M=2m$. [Parallel transport](../../../../../parallel-transport.md) around the closed geodesic preserves the metric and orientation, so lies in the [special orthogonal group](../../../../../special-orthogonal-group.md). It fixes the nonzero tangent $T$, and its restriction to $T^\perp$ is an orientation-preserving orthogonal map of odd dimension $2m-1$. An [odd-dimensional special orthogonal transformation has a fixed vector](../../../../../odd-dimensional-special-orthogonal-transformation-has-a-fixed-vector.md): nonreal eigenvalues occur in conjugate pairs, while an odd-dimensional real orthogonal map with determinant one must have an eigenvalue $+1$. Choose a nonzero fixed vector $v$ normal to $T$ and parallel-transport it along the curve. It gives a nonzero smooth periodic normal field $V$ with $\nabla_tV=0$.

For the exponential variation $\gamma_s(t)=\exp_{\gamma(t)}(sV(t))$, the endpoints match periodically. Strictly positive [sectional curvature](../../../../../sectional-curvature.md) gives

$$
E''(0)=-\int\langle R(V,T)T,V\rangle\,dt<0,\qquad E'(0)=0.
$$

Thus $E(\gamma_s)<E(\gamma)$ for small nonzero $s$. By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md),

$$
L(\gamma_s)^2\leq2(b-a)E(\gamma_s)
<2(b-a)E(\gamma)=L(\gamma)^2,
$$

where the final equality uses the geodesic's constant speed. This proves the [instability of a closed geodesic in positive even-dimensional curvature](../../../../../instability-of-a-closed-geodesic-in-positive-even-dimensional-curvature.md).

For an embedded closed geodesic, sufficiently small variations remain embeddings, hence give a [smooth isotopy](../../../../../smooth-isotopy.md) with strictly shorter curves. For a nonembedded closed geodesic the construction gives a smooth deformation through immersions; an isotopy class of embeddings is not literally defined for such a curve. The stated isotopy conclusion therefore uses the usual embedded-curve interpretation, while the shorter-loop variation holds without it.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 115](../../paper-115-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
