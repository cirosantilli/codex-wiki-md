<h1 id="12/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A forced plain choice occurs exactly when the last chocolate is taken before the final Fellow is served: if it is taken by choice $f\leq F-1$, choice $f+1$ has no chocolate available, whatever that person's preference would have been. Exhaustion precisely on choice $F$ forces nobody. The distinct possible exhaustion times are disjoint events, hence

$$
\boxed{P_{\rm Disaster}=\sum_{f=C}^{F-1}\binom{f-1}{C-1}p^C(1-p)^{f-C}.}
$$

Equivalently, imagine independent preferred choices even after stock is exhausted. The event is that at least $C$ preferred chocolate choices occur among the first $F-1$ people, so the [binomial distribution](../../../../../../binomial-distribution.md) gives $P_{\rm Disaster}=\sum_{k=C}^{F-1}\binom{F-1}{k}p^k(1-p)^{F-1-k}$. The [success-count and waiting-time duality](../../../../../../success-count-and-waiting-time-duality.md) explains equality of these two sums. Plain-biscuit depletion cannot interfere because $D>F$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
