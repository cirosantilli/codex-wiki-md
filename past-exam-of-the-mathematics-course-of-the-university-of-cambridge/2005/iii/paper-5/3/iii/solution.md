<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $U_\alpha=\{x:m_u(f)(x)>\alpha\}$. It is open: it is the union of all [open intervals](../../../../../../open-interval.md) $I$ for which $\int_I|f|>\alpha|I|$. This also proves [measurability](../../../../../../measurability.md) of the [uncentered maximal function](../../../../../../uncentered-maximal-function-of-a-finite-measure.md). [Triangle inequality](../../../../../../triangle-inequality.md) inside each average proves sublinearity and absolute homogeneity.

Take a [compact subset](../../../../../../compact-space.md) $K\subset U_\alpha$, and choose finitely many such intervals covering it. The one-dimensional [Wiener covering lemma](../../../../../../wiener-covering-lemma.md) selects pairwise disjoint intervals $I_1,\ldots,I_N$ whose concentric triples cover $K$. For a finite family this follows by choosing a longest remaining interval and discarding all intervals intersecting it: each discarded interval has no greater length and lies in the triple of the chosen one. Thus

$$
\lambda(K)\leq3\sum_{j=1}^N|I_j|
<\frac3\alpha\sum_{j=1}^N\int_{I_j}|f|
\leq\frac3\alpha\|f\|_1.
$$

Taking the supremum over [compact subsets](../../../../../../compact-space.md), by [inner regularity of Lebesgue measure](../../../../../../inner-regularity-of-lebesgue-measure.md), gives

$$
\boxed{\lambda\{m_u(f)>\alpha\}\leq
\frac3\alpha\|f\|_1.}
$$

This establishes [weak type (1,1)](../../../../../../weak-type-1-1.md). It is the one-dimensional [uncentered maximal weak-type inequality](../../../../../../uncentered-maximal-weak-type-inequality.md) for the [finite measure](../../../../../../finite-measure.md) $|f(t)|\,dt$; the constant need not be optimal for this question.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
