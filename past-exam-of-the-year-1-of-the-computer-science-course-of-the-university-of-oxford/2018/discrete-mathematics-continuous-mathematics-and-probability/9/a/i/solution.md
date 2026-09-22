<h1 id="9/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a nonnegative integer-valued [random variable](../../../../../../random-variable-split.md), its [probability generating function](../../../../../../probability-generating-function.md) is $G_X(s)=\mathbb E[s^X]=\sum_{k\geq0}\mathbb P(X=k)s^k$, at least for $|s|\leq1$. Insert the [Poisson distribution](../../../../../../poisson-distribution.md) masses and sum the [exponential series](../../../../../../exponential-series.md):

$$
G_X(s)=e^{-\mu}\sum_{k=0}^\infty\frac{(\mu s)^k}{k!}=\boxed{e^{\mu(s-1)}}.
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
