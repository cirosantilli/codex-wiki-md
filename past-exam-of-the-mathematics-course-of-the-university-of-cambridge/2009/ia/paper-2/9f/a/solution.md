<h1 id="9f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual assumption that the two die scores are [independent random variables](../../../../../../independent-random-variables.md). A fair score has [expected value](../../../../../../expected-value.md) $7/2$ and [variance](../../../../../../variance-split.md) $35/12$. [Linearity of expectation](../../../../../../linearity-of-expectation.md) and the [variance of a sum](../../../../../../variance-of-a-sum.md) therefore give

$$
\boxed{\mathbb EX=7,\quad\mathbb EY=0,\quad
\operatorname{Var}X=\operatorname{Var}Y=\frac{35}{6}.}
$$

Count the ordered pairs of scores to obtain the [probability mass functions](../../../../../../probability-mass-function.md)

$$
P(X=x)=\frac{6-|x-7|}{36},\quad x=2,\ldots,12;\qquad
P(Y=y)=\frac{6-|y|}{36},\quad y=-5,\ldots,5.
$$

On these attainable [probability supports](../../../../../../support-of-a-probability-distribution.md), **the maxima occur at $x=7$ and $y=0$, each with probability $1/6$; the minima occur at $x=2,12$ and $y=-5,5$, each with probability $1/36$**. Outside the respective [probability support](../../../../../../support-of-a-probability-distribution.md), the mass is zero.

They are not independent: $Y=0$ implies equal die scores and hence $X$ is an [even number](../../../../../../even-number.md), so $P(X=7,Y=0)=0$, whereas $P(X=7)P(Y=0)=1/36>0$. In fact $\operatorname{Cov}(X,Y)=\operatorname{Var}(S_1)-\operatorname{Var}(S_2)=0$: this is an example of [uncorrelated random variables](../../../../../../uncorrelated-random-variables.md) that are dependent.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
