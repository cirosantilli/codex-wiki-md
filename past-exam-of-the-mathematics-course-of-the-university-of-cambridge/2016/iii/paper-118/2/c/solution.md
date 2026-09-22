<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\pi_i:\mathbb C^{g_i}\to X_i$ be the quotient [covering maps](../../../../../../covering-space.md). Since the source universal cover is [simply connected](../../../../../../simply-connected-space.md), the [lifting criterion for a covering space](../../../../../../lifting-criterion-for-a-covering-space.md) gives a lift $F:\mathbb C^{g_1}\to\mathbb C^{g_2}$ of $f\circ\pi_1$. The lift is a [holomorphic map](../../../../../../holomorphic-map.md) because $\pi_2$ is locally a [biholomorphism](../../../../../../biholomorphism.md).

For every $\lambda\in\Lambda_1$, the difference $F(z+\lambda)-F(z)$ belongs to the discrete [Euclidean lattice](../../../../../../euclidean-lattice.md) $\Lambda_2$. It is a continuous function of $z$ on a [connected](../../../../../../connected-space.md) space, hence is constant. Differentiating shows that each coefficient of $DF$ is $\Lambda_1$-periodic. Such a coefficient is bounded on a compact fundamental parallelepiped, and periodicity bounds it on all of $\mathbb C^{g_1}$. The several-variable [Liouville theorem](../../../../../../liouville-theorem.md), obtained by applying the one-variable theorem on coordinate lines, makes every coefficient constant.

Consequently $DF=A$ for a constant [complex-linear map](../../../../../../complex-linear-map.md) $A$ and $F(z)=Az+x$. The period differences become $A\lambda\in\Lambda_2$. Thus the [affine lift of a holomorphic map between complex tori](../../../../../../affine-lift-of-a-holomorphic-map-between-complex-tori.md) gives

$$
\boxed{f(z+\Lambda_1)=Az+x+\Lambda_2,\qquad A\Lambda_1\subseteq\Lambda_2.}
$$

**Every holomorphic map between complex tori is a homomorphism followed by a translation.** The translation vector $x=F(0)$ is determined modulo $\Lambda_2$, while $A$ is the derivative of any lift and is unaffected by that ambiguity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
