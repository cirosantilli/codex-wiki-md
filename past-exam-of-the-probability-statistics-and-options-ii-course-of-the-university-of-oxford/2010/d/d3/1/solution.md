<h1 id="d/d3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Apply [monotone convergence](../../../../../monotone-convergence-theorem.md) to $A_n=\sum_{k=1}^n|a_k|$. Its limit $A=\sum_{k\ge1}|a_k|$ has integral $\sum_k\int|a_k|<\infty$, so $A<\infty$ [almost everywhere](../../../../../almost-everywhere.md). Thus the original series converges absolutely [almost everywhere](../../../../../almost-everywhere.md). Its partial sums are [bounded](../../../../../boundedness.md) in absolute value by the [integrable function](../../../../../lebesgue-integrable-function.md) $A$, and their limit $s$ satisfies $|s|\le A$. [Dominated convergence](../../../../../dominated-convergence-theorem.md) gives

$$
\boxed{\int s=\lim_n\sum_{k=1}^n\int a_k=\sum_{k=1}^{\infty}\int a_k.}
$$

Assigning any value on the null exceptional set defines an [integrable](../../../../../integrability.md) representative of $s$.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [D3](../../d3.md)
3. [D](../../../d.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
