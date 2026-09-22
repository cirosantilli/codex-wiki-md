<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [tangent vector](../../../../../tangent-vector.md) at $p$ is a [derivation at a point](../../../../../derivation-at-a-point.md): a real-linear map $v:C_p^\infty(M)\to\mathbb R$ on [germs](../../../../../germ-of-a-sheaf-section.md) of smooth functions satisfying

$$
v(fh)=f(p)v(h)+h(p)v(f).
$$

Addition and scalar multiplication preserve this identity, defining the [tangent space](../../../../../tangent-space.md) $T_pM$ as a [vector space](../../../../../vector-space-split.md). A derivation annihilates constants. In a [manifold chart](../../../../../manifold-chart.md) $x=(x^1,\ldots,x^n)$ centered near $p$, the local factorization $f-f(p)=\sum_i(x^i-x^i(p))f_i$, with $f_i(p)=\partial_i f(p)$, gives $v(f)=\sum_iv(x^i)\partial_i f(p)$. The factorization follows by integrating the first derivatives along a straight segment in a sufficiently small coordinate ball. Therefore

$$
\boxed{v=\sum_{i=1}^n v^i\partial_i|_p,\qquad v^i=v(x^i),\qquad\dim T_pM=n.}
$$

Conversely these coordinate derivatives satisfy the derivation identity, so they really give a basis rather than merely a spanning family.

The [cotangent space](../../../../../cotangent-space.md) is the [dual vector space](../../../../../linear-functional.md) $T_p^*M=(T_pM)^*$. Its basis $dx^i|_p$ is characterized by $dx^i(\partial_j)=\delta^i_j$. If $\alpha=a_i dx^i=b_jdy^j$, the [chain rule](../../../../../chain-rule.md) gives the [cotangent coordinate transition](../../../../../cotangent-coordinate-transition.md)

$$
\boxed{b_j=\sum_i a_i\frac{\partial x^i}{\partial y^j}(p).}
$$

The [cotangent bundle](../../../../../cotangent-bundle.md) is the disjoint union $T^*M=\coprod_{p\in M}T_p^*M$, with projection $\pi(p,\alpha)=p$. For each base [manifold chart](../../../../../manifold-chart.md) $(U,x)$, define

$$
\Phi_x:\pi^{-1}U\longrightarrow x(U)\times\mathbb R^n,\qquad(p,a_i dx^i|_p)\longmapsto(x(p),a_1,\ldots,a_n).
$$

Its inverse sends $(z,a)$ to $(x^{-1}(z),a_i dx^i|_{x^{-1}(z)})$. On overlaps the transition is $(x,a)\mapsto(y(x),b)$, with the displayed fibre-linear transformation. Its coefficients and inverse are smooth, so these maps give a [smooth atlas](../../../../../smooth-atlas.md) in dimension $2n$. Give the total space the topology obtained by transporting the product topology through these charts. Different base points are separated by disjoint base neighborhoods; distinct points over the same base point are separated within one bundle chart. A countable base [smooth atlas](../../../../../smooth-atlas.md) and countable product bases give second countability. Thus the total space is a Hausdorff, second-countable [smooth manifold](../../../../../smooth-manifold.md). The same charts are [vector bundle trivializations](../../../../../vector-bundle-trivialization.md), since $\pi$ is product projection and their fibre changes are invertible linear maps.

The intrinsic [canonical one-form on a cotangent bundle](../../../../../canonical-one-form-on-a-cotangent-bundle.md) is

$$
\lambda_{(p,\alpha)}(W)=\alpha(d\pi_{(p,\alpha)}W).
$$

In the bundle chart it is $\lambda=\sum_i a_i dx^i$. This definition is coordinate independent, hence its [exterior derivative](../../../../../exterior-derivative.md) is the globally defined smooth [differential two-form](../../../../../2-form.md)

$$
\boxed{\eta=d\lambda=\sum_i da_i\wedge dx^i.}
$$

This sign follows the fibre-first order in this problem; the equally common position-first [symplectic form](../../../../../symplectic-form.md) is $-d\lambda$. The [volume form](../../../../../volume-form.md)

$$
\eta^n=n!\,da_1\wedge dx^1\wedge\cdots\wedge da_n\wedge dx^n
$$

never vanishes. A smooth manifold is orientable exactly when it admits a nowhere-zero top-degree form; its positive ordered bases determine a consistent [orientation](../../../../../orientation-of-a-simplex.md). Consequently **$T^*M$ is an [orientable smooth manifold](../../../../../orientable-smooth-manifold.md), even when $M$ is not**. This is [cotangent bundle orientation](../../../../../cotangent-bundle-orientation.md). In dimension zero the same conclusion uses the nowhere-zero zero-form $1$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
