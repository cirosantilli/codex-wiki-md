<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $X=m$, the first $m-1$ digits must all differ from $3$ and the next digit must be $3$. [Independence](../../../../../../independent-random-variables.md) gives

$$
\boxed{\mathbb P(X=m)=\left(\frac23\right)^{m-1}\frac13,\qquad m=1,2,\ldots.}
$$

Thus $X$ has the [geometric distribution](../../../../../../geometric-distribution.md) counting trials up to and including the first success, with success [probability](../../../../../../probability.md) $1/3$. For completeness, its [mean](../../../../../../expected-value-split.md) follows from the [tail-sum formula](../../../../../../tail-sum-formula.md):

$$
\mathbb E[X]=\sum_{n=0}^{\infty}\mathbb P(X>n)=\sum_{n=0}^{\infty}\left(\frac23\right)^n=\boxed{3}.
$$

The sum of the [geometric series](../../../../../../geometric-series.md) also proves finiteness of this [expectation](../../../../../../expected-value-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
