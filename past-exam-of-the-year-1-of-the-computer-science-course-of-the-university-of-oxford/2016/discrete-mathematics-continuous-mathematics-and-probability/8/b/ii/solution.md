<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Summing a [geometric series](../../../../../../geometric-series.md) gives the [probability generating function](../../../../../../probability-generating-function.md) of the zero-based [geometric distribution](../../../../../../geometric-distribution.md):

$$
\boxed{G_N(s)=\sum_{j=0}^\infty p(1-p)^js^j=\frac p{1-(1-p)s}.}
$$

The series converges for $|(1-p)s|<1$, in particular on $[0,1]$. At $p=1/2$, $G_N(s)=1/(2-s)$, $G_N'(s)=(2-s)^{-2}$, and $G_N''(s)=2(2-s)^{-3}$. The [factorial moment](../../../../../../factorial-moment.md) identities give $\mathbb E(N)=G_N'(1)=1$ and $\mathbb E[N(N-1)]=G_N''(1)=2$. Thus

$$
\boxed{\mathbb E(N)=1,\qquad\operatorname{Var}(N)=G_N''(1)+G_N'(1)-[G_N'(1)]^2=2.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
