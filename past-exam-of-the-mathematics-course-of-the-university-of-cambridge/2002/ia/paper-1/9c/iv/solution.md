<h1 id="9c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $S_N=\sum_{k=1}^Na_k$, with $S_0=0$. The indices in the $n$th dyadic block have one sign, so

$$
\left|S_{2^{n+1}-1}-S_{2^n-1}\right|
=\sum_{r=0}^{2^n-1}\frac1{2^n+r}>\frac{2^n}{2^{n+1}}=\frac12.
$$

A convergent [sequence](../../../../../../sequence.md) of [partial sums](../../../../../../partial-sum.md) must be a [Cauchy sequence](../../../../../../cauchy-sequence.md): for every $\varepsilon>0$, all sufficiently late pairs of [partial sums](../../../../../../partial-sum.md) differ by less than $\varepsilon$. The displayed differences violate this necessary condition with $\varepsilon=1/4$, at arbitrarily late endpoints. Thus **the [series](../../../../../../series-mathematics.md) diverges**, even though its individual terms tend to zero. This [dyadic-block alternation of reciprocal terms](../../../../../../dyadic-block-alternation-of-reciprocal-terms.md) has growing block lengths; the fixed-length block argument of the previous part does not apply.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [9C](../../9c.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ia](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
