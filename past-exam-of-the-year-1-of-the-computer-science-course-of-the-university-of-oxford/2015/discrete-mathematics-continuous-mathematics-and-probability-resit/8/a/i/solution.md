<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [probability generating function](../../../../../../probability-generating-function.md) of a nonnegative [integer](../../../../../../integer-split.md)-valued [random variable](../../../../../../random-variable-split.md) is

$$
\boxed{G_X(s)=\mathbb E[s^X]=\sum_{k=0}^{\infty}p_X(k)s^k,}
$$

using $s^0=1$ also at $s=0$. It is always defined for $0\leq s\leq1$, and indeed the [power series](../../../../../../power-series.md) converges absolutely for all real or complex $s$ with $|s|\leq1$, because

$$
\sum_{k=0}^{\infty}p_X(k)|s|^k\leq\sum_{k=0}^{\infty}p_X(k)=1.
$$

It may be defined beyond the unit disk where this [power series](../../../../../../power-series.md) converges absolutely; such a larger [domain](../../../../../../domain-mathematical-analysis.md) depends on the [distribution](../../../../../../distribution-mathematical-analysis.md). In particular $G_X(0)=\mathbb P(X=0)$ and $G_X(1)=1$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
