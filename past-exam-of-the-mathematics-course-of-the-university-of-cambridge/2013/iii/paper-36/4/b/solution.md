<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $T=P_{V^\perp}|_U:U\longrightarrow V^\perp$. Positivity of the [directed subspace angle](../../../../../../directed-subspace-angle.md) cosine gives

$$
\|Tu\|\ge\cos\theta_{U,V^\perp}\,\|u\|,
$$

so $T$ is [injective](../../../../../../injective-function.md). The two [vector spaces](../../../../../../vector-space-split.md) have the same finite [dimension](../../../../../../dimension-vector-space.md), $n$. By the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md), $T$ is also [surjective](../../../../../../surjective-function.md). There is no need to assume a second positive [directed subspace angle](../../../../../../directed-subspace-angle.md) cosine in this finite-dimensional case.

For any $f\in H$, find $u\in U$ with $Tu=P_{V^\perp}f$. Then $f-u\in V$. If $u\in U\cap V$, then $Tu=0$, and [injectivity](../../../../../../injective-function.md) gives $u=0$. **Hence**

$$
\boxed{H=U\oplus V.}
$$

The [direct sum](../../../../../../direct-sum.md) is again bounded: $u=T^{-1}P_{V^\perp}f$. If $n=0$, then $U=\{0\}$ and $V^\perp=\{0\}$, so closedness of $V$ gives $V=H$ and the conclusion directly; no angle of an empty unit sphere is needed. Equal finite [dimensions](../../../../../../dimension-vector-space.md) are essential to the surjectivity argument, whereas mere [injectivity](../../../../../../injective-function.md) between infinite-dimensional [Hilbert spaces](../../../../../../hilbert-space-split.md) is insufficient.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
