<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $r$ be the number at risk just after $a$, and suppose the $d$ events are grouped into tie sizes $d_1,\ldots,d_m$ at ordered times in $(a,b]$. With no intervening censoring or entry, their risk counts are $r$, $r-d_1$, $r-d_1-d_2$, and so on. Hence the [Kaplan–Meier telescoping across a censor-free interval](../../../../../../kaplan-meier-telescoping-across-a-censor-free-interval.md) gives

$$
\frac{\widehat F(b)}{\widehat F(a)}
=\prod_{j=1}^m
\frac{r-\sum_{k\leq j}d_k}{r-\sum_{k<j}d_k}
=\frac{r-d}{r},
\qquad
\boxed{\widehat F(b)=\widehat F(a)\frac{r-d}{r}.}
$$

Only the total $d$ appears. Consequently **the order of the events and their grouping into ties do not affect the estimate at $b$**. Censoring exactly at $b$ does not change this conclusion when it is processed after the events at that time, as in the standard convention. The calculation assumes $r>0$; no estimator beyond an exhausted [risk set](../../../../../../risk-set.md) is being inferred from unobserved follow-up.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
