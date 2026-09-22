<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Here closed oriented surfaces are connected, as in the usual single-genus convention. Let $f:X\to Y$ have nonzero [mapping degree](../../../../../degree-of-a-continuous-mapping.md) $d$. Work over $\mathbb Q$, so multiplication by $d$ is invertible and cannot vanish.

The [Poincare duality pairing](../../../../../poincare-duality-pairing.md) on $H^1(Y;\mathbb Q)$ is nondegenerate. Thus for every $0\ne a\in H^1(Y;\mathbb Q)$ there is $b\in H^1(Y;\mathbb Q)$ with $\langle a\smile b,[Y]\rangle\ne0$. Naturality of the [cup product](../../../../../cup-product.md) and evaluation on the [fundamental class](../../../../../fundamental-class.md) give

$$
\langle f^*a\smile f^*b,[X]\rangle
=\langle f^*(a\smile b),[X]\rangle
=\langle a\smile b,f_*[X]\rangle
=d\langle a\smile b,[Y]\rangle\ne0.
$$

In particular $f^*a\ne0$, so $f^*:H^1(Y;\mathbb Q)\to H^1(X;\mathbb Q)$ is injective. The [cohomology ring of a closed oriented surface](../../../../../cohomology-ring-of-a-closed-oriented-surface.md) has $\dim H^1(\Sigma_g;\mathbb Q)=2g$. Comparing dimensions now gives

$$
2g(Y)\le2g(X),\qquad\boxed{g(X)\ge g(Y).}
$$

This proves [genus monotonicity under nonzero-degree surface maps](../../../../../genus-monotonicity-under-nonzero-degree-surface-maps.md) by [rational cohomology injectivity of a nonzero-degree map](../../../../../rational-cohomology-injectivity-of-a-nonzero-degree-map.md), without requiring $f$ to be a covering map or a smooth map.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
