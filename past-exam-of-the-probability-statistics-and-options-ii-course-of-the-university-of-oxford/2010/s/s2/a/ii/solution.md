<h1 id="s/s2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For one trial and any measurable set $A$,

$$
P(Y\in A,\text{accept})=\int_Aq(y)\frac{p(y)}{Mq(y)}dy=\frac1M\int_Ap(y)dy.
$$

Since the acceptance probability is $1/M$, conditioning gives target probability $\int_Ap$. Repeating failed [independent](../../../../../../independent-random-variables.md) trials does not alter this conditional law: summing over the trial number multiplies by the geometric sum $\sum_{j\ge0}(1-1/M)^j/M=1$. Taking $A=(-\infty,x)$ proves

$$
\boxed{P(X<x)=\int_{-\infty}^xp(y)dy.}
$$

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [S2](../../../s2.md)
4. [S](../../../../s.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
