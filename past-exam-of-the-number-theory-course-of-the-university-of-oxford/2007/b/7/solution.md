<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

[Minkowski convex body theorem](../../../../minkowski-s-theorem.md) states that a centrally symmetric [convex](../../../../convex-function.md) measurable subset of $\mathbb R^n$ with [volume](../../../../volume.md) greater than $2^n$ times the [covolume](../../../../covolume.md) of a full [Euclidean lattice](../../../../euclidean-lattice.md) contains a nonzero lattice point. The equivalent closed-boundary form follows by compactness for compact [convex](../../../../convex-function.md) bodies.

The set $S_t$ is centrally symmetric. It is [convex](../../../../convex-function.md) because for $0\le\lambda\le1$, the [triangle inequality](../../../../triangle-inequality.md) gives $\|\lambda u+(1-\lambda)v\|_1\le\lambda\|u\|_1+(1-\lambda)\|v\|_1\le t$. It is a diamond of area $2t^2$. For the embedded nonzero [integral ideal](../../../../integral-ideal.md) $I$, the given [covolume](../../../../covolume.md) is $2N(I)\sqrt d$. Hence [Minkowski convex body theorem](../../../../minkowski-s-theorem.md) applies when

$$
2t^2>8N(I)\sqrt d,\qquad t^2>4N(I)\sqrt d.
$$

For the resulting nonzero $\alpha\in I$, write $x=\sigma_1(\alpha)$, $y=\sigma_2(\alpha)$. Then

$$
|\operatorname{Norm}_{K/\mathbb Q}(\alpha)|=|xy|
\le\frac{(|x|+|y|)^2}{4}\le\frac{t^2}{4}.
$$

Decrease $t$ to $2\sqrt{N(I)\sqrt d}$. A fixed slightly larger diamond contains only finitely many lattice points, so one nonzero $\alpha$ recurs along a sequence of such $t$ values. Passing to the limit proves

$$
\boxed{|\operatorname{Norm}_{K/\mathbb Q}(\alpha)|\le N(I)\sqrt d.}
$$

Given a target [ideal class](../../../../ideal-class.md) $C$, choose an [integral ideal](../../../../integral-ideal.md) $I$ in $C^{-1}$. Since $\alpha\in I$, the [ideal](../../../../ideal.md) $J=(\alpha)I^{-1}$ is integral, belongs to $C$, and has [ideal norm](../../../../ideal-norm.md)

$$
N(J)=\frac{|\operatorname{Norm}(\alpha)|}{N(I)}\le\sqrt d.
$$

For $K=\mathbb Q(\sqrt{14})$, every [ideal class](../../../../ideal-class.md) thus has an integral representative of norm at most $\sqrt{14}<4$. The only possibilities are norms one, two or three. The prime two ramifies, giving the unique [ideal](../../../../ideal.md) of norm two $P_2=(2,\sqrt{14})$. The element $4+\sqrt{14}$ has [field norm](../../../../field-norm.md) $16-14=2$, so $(4+\sqrt{14})=P_2$, making it principal. The prime three is inert because $X^2-14\equiv X^2+1\pmod3$ is an [irreducible polynomial](../../../../irreducible-polynomial.md); its [prime ideal](../../../../prime-ideal.md) has norm nine, so there is no [ideal](../../../../ideal.md) of norm three. Every possible small representative is principal, proving [class number one for Q square root of fourteen](../../../../class-number-one-for-q-square-root-of-fourteen.md). Therefore

$$
\boxed{h(\mathbb Q(\sqrt{14}))=1.}
$$

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
