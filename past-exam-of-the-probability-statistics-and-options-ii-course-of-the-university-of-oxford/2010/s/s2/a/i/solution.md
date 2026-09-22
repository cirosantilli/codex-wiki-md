<h1 id="s/s2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Independently draw $Y\sim q$ and $U\sim\operatorname{Uniform}(0,1)$. Accept $Y$ if $U\le p(Y)/(Mq(Y))$; otherwise discard it and repeat with fresh [independent](../../../../../../independent-random-variables.md) draws. Return the first accepted value. The bound makes the acceptance probability at each proposal at most one. As $\int p=1$, the total acceptance probability is $1/M>0$, so the procedure terminates almost surely. Values outside the proposal support must have target [density](../../../../../../probability-density-function.md) zero for the stated envelope assumption to make sense.

## ↑ Ancestors (14)

1. [I](../i.md)
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
