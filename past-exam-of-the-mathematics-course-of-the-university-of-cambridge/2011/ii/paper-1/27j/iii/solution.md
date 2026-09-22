<h1 id="27j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Starting from $+1$, the level reaches $c$ at time $c$ if the first holding time exceeds $c$. This has probability $e^{-ac}$; surviving beyond $c$ also makes the level strictly greater than $c$, as required by the strict event. A switch to $-1$ at time $u<c$ has density $qe^{-au}\,du$, leaves level $u$, and requires a later rise of $c-u$. Absorption before reaching $c$ cannot succeed. Therefore

$$
\boxed{\psi_+(c)=e^{-(q+\lambda)c}+\int_0^cqe^{-(q+\lambda)u}\psi_-(c-u)\,du.}
$$

Holding times have continuous distributions, so the single endpoint $u=c$ has no effect on the formula.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [27J](../../27j.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
