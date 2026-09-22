<h1 id="17/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $p=P(A)$ and $q=P(B\mid A)$. Decompose the marginal as $P(B)=P(A\cap B)+P(A^c\cap B)=pq+t$, where $0\leq t\leq1-p$. It follows that

$$
\boxed{pq\leq P(B)\leq pq+1-p}.
$$

Both bounds are attainable: choose none or all of the mass outside $A$ to belong to $B$. More explicitly, the four joint cell masses can be $pq,p(1-q),t,1-p-t$, all nonnegative. This is the first case of [sharp bounds from binary conditional probabilities](../../../../../../sharp-bounds-from-binary-conditional-probabilities.md).

For the usual conditional-probability ratio, the given $q$ requires $p>0$. If $p=1$, the two bounds coincide at $q$. If $p=0$, the conditional is undefined as a ratio, although its formal joint-model bounds reduce to $0\leq P(B)\leq1$.

## ↑ Ancestors (14)

1. [I](../i.md)
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
