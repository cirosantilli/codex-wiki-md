<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $D_i$ be the result of roll $i$, so $X=\sum_{i=1}^{100}D_i$. Each $D_i$ has the [uniform distribution on a finite set](../../../../../discrete-uniform-distribution.md) $\{1,\ldots,6\}$, giving

$$
\mathbb E D_i=\frac{1+2+3+4+5+6}{6}=\frac72,
\qquad
\mathbb E D_i^2=\frac{1+4+9+16+25+36}{6}=\frac{91}{6},
$$

and hence [variance](../../../../../variance-split.md) $\operatorname{Var}(D_i)=91/6-(7/2)^2=35/12$. The rolls are [independent](../../../../../independent-random-variables.md), so [linearity of expectation](../../../../../linearity-of-expectation.md) and [variance additivity for independent random variables](../../../../../variance-additivity-for-independent-random-variables.md) give

$$
\mathbb E X=350,
\qquad
\operatorname{Var}(X)=100\frac{35}{12}=\frac{875}{3}.
$$

All the required [moments](../../../../../moment.md) are finite. Taking $a=50$ in [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md) now yields

$$
\boxed{\mathbb P(|X-350|\geq50)\leq\frac{875/3}{2500}=\frac7{60}\approx0.1167.}
$$

This is an upper bound, rather than an exact tail [probability](../../../../../probability.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
