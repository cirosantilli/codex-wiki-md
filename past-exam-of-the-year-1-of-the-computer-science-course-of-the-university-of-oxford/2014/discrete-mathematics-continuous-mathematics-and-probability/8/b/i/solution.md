<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Given $X=k$, the score $Y$ has a [binomial distribution](../../../../../../binomial-distribution.md) with success [probability](../../../../../../probability.md) $1/2$. Its conditional [expected value](../../../../../../expected-value-split.md) and [variance](../../../../../../variance-split.md) are $k/2$ and $k/4$. Thus

$$
\boxed{\mathbb E[Y\mid X=k]=\frac k2,\qquad
\mathbb E[Y^2\mid X=k]=\frac k4+\frac{k^2}{4}.}
$$

This is [binomial thinning](../../../../../../binomial-thinning.md) of the first-round count; the second formula uses the identity $\mathbb E[Y^2\mid X]=\operatorname{Var}(Y\mid X)+\mathbb E[Y\mid X]^2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
