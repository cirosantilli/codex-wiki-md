<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each $N\geq1$, put $C_N=\bigcup_{n\geq N}A_n$. Closure of a [sigma-algebra](../../../../../sigma-algebra.md) under [countable unions](../../../../../countable-union.md) and [countable intersections](../../../../../countable-intersection.md) gives

$$
A=\limsup_{n\to\infty}A_n=\bigcap_{N\geq1}C_N\in\mathcal F.
$$

The [events](../../../../../event.md) $C_N$ decrease to $A$. [Continuity of probability](../../../../../continuity-of-probability.md) from above applies because $\mathbb P(C_1)\leq1<\infty$. Also, $A_n\subseteq C_N$ whenever $n\geq N$, so

$$
\mathbb P(C_N)\geq\sup_{n\geq N}\mathbb P(A_n).
$$

Letting $N\to\infty$ proves

$$
\boxed{\mathbb P(A)=\lim_{N\to\infty}\mathbb P(C_N)
\geq\lim_{N\to\infty}\sup_{n\geq N}\mathbb P(A_n)
=\limsup_{n\to\infty}\mathbb P(A_n).}
$$

This [reverse Fatou inequality for events](../../../../../reverse-fatou-inequality-for-events.md) requires no [independence](../../../../../independent-random-variables.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
