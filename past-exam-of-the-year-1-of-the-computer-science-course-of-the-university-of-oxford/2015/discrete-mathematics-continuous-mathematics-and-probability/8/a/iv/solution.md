<h1 id="8/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For the [Poisson distribution](../../../../../../poisson-distribution.md) with parameter $1$, the [exponential series](../../../../../../exponential-series.md) gives

$$
G(s)=\sum_{j=0}^{\infty}\frac{e^{-1}s^j}{j!}
=\boxed{e^{s-1}},\qquad s\in\mathbb R.
$$

Every [derivative](../../../../../../derivative.md) is $G^{(k)}(s)=e^{s-1}$, so the [factorial moments](../../../../../../factorial-moment.md) are

$$
\boxed{\mathbb E[X(X-1)\cdots(X-k+1)]=1\qquad(k\ge0).}
$$

In particular $G'(1)=G''(1)=1$, and the [variance](../../../../../../variance-split.md) is

$$
\boxed{\operatorname{var}(X)=1+1-1^2=1.}
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
