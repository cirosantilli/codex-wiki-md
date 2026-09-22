<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $B$ count the red balls among the $n$ added balls. By [independence of random variables](../../../../../../independent-random-variables.md), $B$ has a [binomial distribution](../../../../../../binomial-distribution.md) with parameters $n,1/2$. The total red count is $R=1+B$, and the box has $n+1$ balls. Conditional on $R=r$, [sampling without replacement](../../../../../../sampling-without-replacement.md) gives

$$
\mathbb P(D_1\mid R=r)=\frac r{n+1},\qquad\mathbb P(D_1\cap D_2\mid R=r)=\frac{r(r-1)}{n(n+1)},
$$

where $D_1,D_2$ denote red first and second draws. Averaging these [conditional probabilities](../../../../../../conditional-probability.md) and taking their ratio gives

$$
\mathbb P(D_2\mid D_1)=\frac{\mathbb E[R(R-1)]}{n\mathbb E[R]}.
$$

The [binomial distribution](../../../../../../binomial-distribution.md) moments give $\mathbb E[B]=n/2$ and $\mathbb E[B^2]=n/4+n^2/4$. Consequently

$$
\mathbb E[R]=\frac{n+2}{2},\qquad\mathbb E[R(R-1)]=\mathbb E[B^2+B]=\frac{n(n+3)}4.
$$

Therefore the [red-ball prediction with one certain red ball](../../../../../../red-ball-prediction-with-one-certain-red-ball.md) is

$$
\boxed{\mathbb P(D_2\mid D_1)=\frac{n+3}{2(n+2)},\qquad n\geq1.}
$$

It reduces to $2/3$ at $n=1$ and approaches $1/2$ as the number of randomly coloured extra balls grows. Taking an unweighted average of the remaining red fractions would miss the change in weights caused by taking a [conditional probability](../../../../../../conditional-probability.md) given the first red draw.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
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
