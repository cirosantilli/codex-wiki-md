<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $T_2$ be the time of the second occurrence of $3$, whether or not it is adjacent to the first. On every digit [sequence](../../../../../../sequence.md), completion of a consecutive pair requires at least two occurrences of $3$, so $Y\geqslant T_2$.

The waiting time for the first $3$ has [mean](../../../../../../expected-value-split.md) $3$. Once that digit has appeared, the fresh independent digits give another waiting time with the same [mean](../../../../../../expected-value-split.md) for the next $3$. Thus $\mathbb E[T_2]=3+3=6$, the [mean](../../../../../../expected-value-split.md) of the corresponding [negative binomial distribution](../../../../../../negative-binomial-distribution.md). Monotonicity of [expectation](../../../../../../expected-value-split.md) now proves **$\mathbb E[Y]\geqslant6$**, without computing the waiting time for the consecutive pair itself. The argument remains valid even before establishing that $Y$ has finite mean, since these waiting times are nonnegative.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
