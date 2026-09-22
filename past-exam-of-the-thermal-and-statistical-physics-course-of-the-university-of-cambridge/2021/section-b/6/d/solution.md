<h1 id="section-b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At the root all $z$ neighbours are in shell one, so the [probability](../../../../../probability.md) of leaving the root for that shell is one. Conversely, a walker anywhere in shell one chooses its unique rootward [edge](../../../../../edge-of-a-graph.md) with [probability](../../../../../probability.md) $1/z$. The two boundary recurrences are therefore

$$
\boxed{P(1,N+1)=P(0,N)+\frac1zP(2,N),}
$$



$$
\boxed{P(0,N+1)=\frac1zP(1,N).}
$$

Together with $P(0,0)=1$ and $P(r>0,0)=0$, these equations determine the distribution. In particular $P(1,1)=1$ and $P(0,2)=1/z$, which check the special root coefficient. For the original indexing, replace $N+1$ by $N$ and $N$ by $N-1$ on the right-hand sides. Summing these equations and the bulk recurrence conserves $\sum_{r\geq0}P(r,N)=1$.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
