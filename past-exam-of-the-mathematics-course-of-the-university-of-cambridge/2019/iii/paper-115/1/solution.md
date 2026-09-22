<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [exterior derivative](../../../../../exterior-derivative.md) is the real-linear degree-one map $d:\Omega^r(M)\to\Omega^{r+1}(M)$ characterized by $df(X)=Xf$ on [smooth functions](../../../../../smooth-function.md), the graded [Leibniz rule](../../../../../leibniz-rule.md)

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^r\alpha\wedge d\beta
\qquad(\alpha\in\Omega^r(M)),
$$

and $d^2=0$. In [local coordinates](../../../../../local-coordinate.md) $(x^1,\ldots,x^m)$, write $\alpha=\sum_I\alpha_I dx^{i_1}\wedge\cdots\wedge dx^{i_r}$ using [multi-index notation](../../../../../multi-index-notation.md). Since $dx^i=d(x^i)$ and hence $d(dx^i)=0$, the defining rules force

$$
\boxed{d\alpha=\sum_{I,j}\frac{\partial\alpha_I}{\partial x^j}dx^j\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_r}.}
$$

This proves local uniqueness, and the coordinate formulas agree on overlaps because the same rules are preserved by the [pullback of a differential form](../../../../../pullback-of-a-differential-form.md). They also directly define an operator satisfying all three rules, proving existence.

An [exact differential form](../../../../../exact-differential-form.md) is a form $\omega=d\eta$. Let $\pi:S^{2n}\to\mathbb{RP}^{2n}$ be the antipodal double [covering map](../../../../../covering-space.md) and let $a(x)=-x$. For a $2n$-form $\omega$ on real projective space, $a^*\pi^*\omega=\pi^*\omega$, while the [mapping degree](../../../../../degree-of-a-continuous-mapping.md) of the [antipodal map](../../../../../antipodal-map.md) is $-1$. Therefore

$$
\int_{S^{2n}}\pi^*\omega
=\int_{S^{2n}}a^*\pi^*\omega
=-\int_{S^{2n}}\pi^*\omega=0.
$$

By the stated criterion, $\pi^*\omega=d\eta$. The [invariant primitive under a finite group action](../../../../../invariant-primitive-under-a-finite-group-action.md)

$$
\bar\eta=\frac12(\eta+a^*\eta)
$$

still satisfies $d\bar\eta=\pi^*\omega$ and descends to a form $\beta$ on $\mathbb{RP}^{2n}$. Since pullback through a covering is injective on differential forms, $\pi^*(d\beta-\omega)=0$ implies $d\beta=\omega$. Thus **every $2n$-form on $\mathbb{RP}^{2n}$ is exact**; this is the [top-degree differential forms on even-dimensional real projective space are exact](../../../../../top-degree-differential-forms-on-even-dimensional-real-projective-space-are-exact.md) result.

The $k$th [de Rham cohomology](../../../../../de-rham-cohomology.md) is

$$
H^k_{\mathrm{dR}}(M)=\frac{\ker(d:\Omega^k(M)\to\Omega^{k+1}(M))}{\operatorname{im}(d:\Omega^{k-1}(M)\to\Omega^k(M))},
$$

the [closed differential forms](../../../../../closed-differential-form.md) modulo the exact ones. For the product, let $p:M\times S^1\to M$ be projection and choose a closed one-form $\nu$ on the circle with $\int_{S^1}\nu=1$. [Averaging differential forms over the circle](../../../../../averaging-differential-forms-over-the-circle.md) is cochain-homotopic to the identity, so every class has a rotation-invariant representative; if such a representative is exact, averaging a primitive gives an invariant primitive. Every invariant $k$-form has a unique decomposition $p^*\alpha+p^*\beta\wedge\nu$, and

$$
d(p^*\alpha+p^*\beta\wedge\nu)=p^*(d\alpha)+p^*(d\beta)\wedge\nu.
$$

Closedness and exactness are therefore componentwise. Hence the map

$$
\boxed{([\alpha],[\beta])\longmapsto[p^*\alpha+p^*\beta\wedge\nu]}
$$

is a well-defined bijection $H^k_{\mathrm{dR}}(M)\oplus H^{k-1}_{\mathrm{dR}}(M)\to H^k_{\mathrm{dR}}(M\times S^1)$, proving the [de Rham cohomology of a product with a circle](../../../../../de-rham-cohomology-of-a-product-with-a-circle.md) formula.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 115](../../paper-115-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
