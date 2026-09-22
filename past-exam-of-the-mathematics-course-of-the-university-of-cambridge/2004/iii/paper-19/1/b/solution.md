<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $D_t=\nabla_{\dot\gamma}$ and let $P_t:T_pM\to T_{\gamma(t)}M$ denote [parallel transport](../../../../../../parallel-transport.md). Since $\gamma$ is a [geodesic](../../../../../../geodesic.md), $D_t\dot\gamma=0$, while the transported vectors satisfy $D_te_i(t)=0$. The [locally symmetric Riemannian manifold](../../../../../../locally-symmetric-riemannian-manifold.md) condition is $\nabla R=0$. Hence the [Levi-Civita connection](../../../../../../levi-civita-connection.md) product rule yields

$$
D_t\bigl(R(\dot\gamma,e_i(t))\dot\gamma\bigr)
=(\nabla_{\dot\gamma}R)(\dot\gamma,e_i(t))\dot\gamma
+R(D_t\dot\gamma,e_i(t))\dot\gamma
+R(\dot\gamma,D_te_i(t))\dot\gamma
+R(\dot\gamma,e_i(t))D_t\dot\gamma=0.
$$

Both this vector field and $\lambda_i e_i(t)$ are parallel and agree at zero. Uniqueness of [parallel transport](../../../../../../parallel-transport.md) therefore proves

$$
\boxed{K_{\dot\gamma(t)}e_i(t)=\lambda_i e_i(t),\qquad K_{\dot\gamma(t)}=P_tK_vP_t^{-1}.}
$$

The [eigenvalues](../../../../../../eigenvalue.md) are independent of $t$. The original PDF has $K_{\dot\gamma(t)}$ here; the converted TeX omits the dot, which would incorrectly put a point rather than a tangent vector in the operator's subscript.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
