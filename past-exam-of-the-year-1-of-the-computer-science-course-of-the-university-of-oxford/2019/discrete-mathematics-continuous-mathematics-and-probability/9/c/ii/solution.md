<h1 id="9/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Every particular card is second with [probability](../../../../../../probability.md)

$$
\sum_{\text{999 other first cards}}\frac1{1000}\frac1{999}
=\frac1{1000}.
$$

Hence **$X$ and $Y$ have the same distribution**, with means zero and variances one. They are not [independent](../../../../../../independent-random-variables.md), since a card cannot be drawn twice.

Every ordered pair of distinct cards has [probability](../../../../../../probability.md) $1/(1000\cdot999)$. Therefore

$$
\begin{aligned}
\operatorname{Cov}(X,Y)=\mathbb E[XY]
&=\frac{\sum_{i\ne j}a_i a_j}{1000\cdot999}\\
&=\frac{(\sum_i a_i)^2-\sum_i a_i^2}{1000\cdot999}
=\boxed{-\frac1{999}}.
\end{aligned}
$$

This negative [covariance](../../../../../../covariance.md) is the effect of [sampling without replacement](../../../../../../sampling-without-replacement.md), not a contradiction of their identical marginals.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
