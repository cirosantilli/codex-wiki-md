<h1 id="17/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $q=P(B\mid A)$, $s=P(B\mid A^c)$ and $p=P(A)$. The [law of total probability](../../../../../../law-of-total-probability.md) gives $P(B)=pq+(1-p)s$, a [convex combination](../../../../../../convex-combination.md) of the two fixed conditional values. Hence

$$
\boxed{\min(q,s)\leq P(B)\leq\max(q,s)}.
$$

These are the closed sharp bounds in the usual mixture-model interpretation, obtained by allowing $p$ to range from zero to one. The joint masses $pq,p(1-q),(1-p)s,(1-p)(1-s)$ realize every such mixture.

There is an endpoint qualification if both conditionals must literally be defined by ratios: then $0<p<1$. If $q\ne s$, the marginal lies strictly between them, so the stated endpoints are an [infimum](../../../../../../infimum.md) and [supremum](../../../../../../supremum.md) rather than achieved extrema. If $q=s$, every allowed mixture has exactly that common value. This is the second case of [sharp bounds from binary conditional probabilities](../../../../../../sharp-bounds-from-binary-conditional-probabilities.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [17](../../../17.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
