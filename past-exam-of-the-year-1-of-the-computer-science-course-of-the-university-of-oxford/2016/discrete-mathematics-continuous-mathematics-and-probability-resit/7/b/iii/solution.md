<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $D$ be the number of days up to and including the first breakdown, and $M$ the event of a morning first breakdown. For $d=1,2,\ldots$, [conditional probability](../../../../../../conditional-probability.md) gives

$$
\mathbb P(D=d\mid M)=\frac{\alpha q^{d-1}}{\alpha/(1-q)}=(1-q)q^{d-1}.
$$

Thus

$$
\boxed{D\mid M\sim\operatorname{Geom}(\alpha+\beta-\alpha\beta)\text{ on }\{1,2,\ldots\}}.
$$

This [geometric distribution](../../../../../../geometric-distribution.md) counts the day on which the first breakdown occurs. Its parameter is the probability of at least one breakdown during a day, rather than the morning breakdown probability $\alpha$ alone.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
