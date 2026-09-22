<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The given four probabilities factor into independent [Bernoulli](../../../../../bernoulli-distribution.md) indicators for the occurrence of $A$ and $B$ on each trial, with parameters $p$ and $r$. Independent trials make the full sequence of $A$ indicators independent of the full sequence of $B$ indicators. Let $N$ count trials strictly before the first $A$. Then $N\sim\operatorname{Geom}_0(p)$, independently of the $B$ indicators, and the desired count is their sum over these $N$ trials. Therefore **its distribution is $\operatorname{Geom}_0(p/[p+(1-p)r])$**, as in part (b).

The word “before” excludes the stopping trial: an $AB$ on that trial stops the experiment but does not add to the count. Another check is to discard all $ab$ trials. Among the remaining relevant outcomes, stopping has probability $p/[p+(1-p)r]$ and an additional pre-stopping $B$ has the complementary probability, again giving the same zero-based [geometric distribution](../../../../../geometric-distribution.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
