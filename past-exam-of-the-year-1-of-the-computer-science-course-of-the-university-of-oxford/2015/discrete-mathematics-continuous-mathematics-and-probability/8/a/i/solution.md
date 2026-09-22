<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [probability generating function](../../../../../../probability-generating-function.md) of a nonnegative [integer-valued random variable](../../../../../../integer-valued-random-variable.md) is

$$
\boxed{G(s)=\mathbb E[s^X]=\sum_{j=0}^{\infty}p(j)s^j.}
$$

Use $s^0=1$, including at $s=0$. The [power series](../../../../../../power-series.md) converges absolutely for every real $s\in[-1,1]$, since $\sum_jp(j)|s|^j\le1$. In particular it is always defined on the usual probability-generating interval $[0,1]$. It may also be defined for $|s|>1$, depending on the [radius of convergence](../../../../../../radius-of-convergence.md) and convergence at its endpoints; the precise real [domain](../../../../../../domain-mathematical-analysis.md) of finite expectation is $\{s\in\mathbb R:\sum_jp(j)|s|^j<\infty\}$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
