<h1 id="8/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [Bernoulli random variable](../../../../../../bernoulli-distribution.md) with parameter $1/2$ has $G_Y(s)=(1+s)/2$. Part (i) and the [geometric distribution](../../../../../../geometric-distribution.md) formula give

$$
G_X(s)=\frac1{2-(1+s)/2}=\frac2{3-s}
=\frac23\sum_{j=0}^\infty\left(\frac s3\right)^j.
$$

Comparing coefficients in the [probability generating function](../../../../../../probability-generating-function.md) identifies

$$
\boxed{\mathbb P(X=j)=\frac23\left(\frac13\right)^j,\quad j=0,1,\ldots.}
$$

Thus **$X$ has the zero-based [geometric distribution](../../../../../../geometric-distribution.md) with success parameter $2/3$**. The probabilities sum to one, and its mean $1/2$ agrees with the random-sum mean $\mathbb E(N)\mathbb E(Y_1)=1\cdot1/2$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
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
