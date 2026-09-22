<h1 id="7/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [binomial distribution](../../../../../../binomial-distribution.md), the [binomial theorem](../../../../../../binomial-theorem.md) gives

$$
G_X(s)=\sum_{k=0}^n\binom nkp^k(1-p)^{n-k}s^k=(1-p+ps)^n.
$$

Differentiation of the [probability generating function](../../../../../../probability-generating-function.md) recovers the first [expected value](../../../../../../expected-value-split.md) and second [factorial moment](../../../../../../factorial-moment.md):

$$
G_X'(1)=np,\qquad G_X''(1)=n(n-1)p^2=\mathbb E[X(X-1)].
$$

Since $X^2=X(X-1)+X$, the [variance](../../../../../../variance-split.md) is

$$
G_X''(1)+G_X'(1)-G_X'(1)^2=n(n-1)p^2+np-n^2p^2=np(1-p).
$$

Thus

$$
\boxed{G_X(s)=(1-p+ps)^n,\qquad\mathbb E[X]=np,\qquad\operatorname{var}(X)=np(1-p).}
$$

The formulas also hold for $n=0,1$ and the degenerate choices $p=0,1$, with derivatives read directly from the resulting [polynomial](../../../../../../polynomial-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
