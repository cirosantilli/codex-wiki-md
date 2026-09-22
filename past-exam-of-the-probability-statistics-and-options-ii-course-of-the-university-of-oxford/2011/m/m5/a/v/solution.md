<h1 id="m/m5/a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let $e_k$ be the expected number of future children receiving stickers from a box containing $k$, with $e_0=0$. Conditioning on the first uniform remainder gives

$$
e_k=1+\frac1k\sum_{j=0}^{k-1}e_j.
$$

Subtract the corresponding identity for $k-1$ after multiplying each by its denominator. This gives $ke_k=k e_{k-1}+1$, so $e_k=e_{k-1}+1/k$. Therefore $e_N=\sum_{j=1}^N1/j$, and

$$
\boxed{e_4=1+\frac12+\frac13+\frac14=\frac{25}{12}.}
$$

The recurrence counts the current positive recipient once and excludes all later children arriving after the box is empty.

## ↑ Ancestors (14)

1. [V](../v.md)
2. [A](../../a.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
