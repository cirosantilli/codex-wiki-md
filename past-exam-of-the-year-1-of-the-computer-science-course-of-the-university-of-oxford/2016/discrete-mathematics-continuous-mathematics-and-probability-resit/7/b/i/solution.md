<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $q=(1-\alpha)(1-\beta)$, the probability of surviving a full day, and $p=1-q=\alpha+\beta-\alpha\beta$. These lie in $(0,1)$. Let $M$ be the event that the first breakdown is in the morning. By [independence](../../../../../../independent-random-variables.md), surviving $d-1$ complete days and then failing in the morning of day $d$ has probability $q^{d-1}\alpha$.

These events are disjoint, so summing the [geometric series](../../../../../../geometric-series.md) gives

$$
\boxed{\mathbb P(M)=\sum_{d=1}^{\infty}\alpha q^{d-1}=\frac\alpha{\alpha+\beta-\alpha\beta}}.
$$

There is no missing probability of never breaking down: survival for $d$ days has probability $q^d\to0$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
