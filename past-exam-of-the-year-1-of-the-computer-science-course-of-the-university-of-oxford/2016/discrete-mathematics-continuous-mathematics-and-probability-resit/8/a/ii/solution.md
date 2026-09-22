<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By definition, the [probability generating function](../../../../../../probability-generating-function.md) is

$$
G_X(s)=\mathbb E(s^X)=\sum_{n=0}^{\infty}s^n\mathbb P(X=n).
$$

Substituting the [Poisson distribution](../../../../../../poisson-distribution.md) and evaluating the [exponential series](../../../../../../exponential-series.md) gives

$$
\boxed{G_X(s)=e^{-\lambda}\sum_{n=0}^{\infty}\frac{(\lambda s)^n}{n!}=e^{\lambda(s-1)}}.
$$

The series converges for every finite complex $s$; in particular it gives the [probability generating function](../../../../../../probability-generating-function.md) on $0\leq s\leq1$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
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
