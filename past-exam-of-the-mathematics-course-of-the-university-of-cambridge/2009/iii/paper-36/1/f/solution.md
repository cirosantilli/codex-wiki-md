<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For the uniform [prior](../../../../../../prior-probability.md), write $s=x+y$ for the pooled success count in $m+n$ trials. Conditional on $s$, exchangeability makes all placements of the successes equally likely. The successes in the second batch therefore have a [hypergeometric distribution](../../../../../../hypergeometric-distribution.md), and the factor in question is

$$
B=\frac{\binom{s}{y}\binom{m+n-s}{n-y}}{\binom{m+n}{n}}
=\Pr(Y=y\mid X+Y=s)\quad\text{at }s=x+y.
$$

This is [hypergeometric allocation of exchangeable Bernoulli counts](../../../../../../hypergeometric-allocation-of-exchangeable-bernoulli-counts.md): sample $n$ positions without replacement from a population of $m+n$ positions containing $s$ successes. The [uniform-count predictive property](../../../../../../uniform-count-predictive-property.md) gives $\Pr(X+Y=s)=1/(m+n+1)$ and $\Pr(X=x)=1/(m+1)$, so

$$
\boxed{\Pr(Y=y\mid X=x)=\frac{m+1}{m+n+1}\,B.}
$$

As $y$ varies with $x$ fixed, $s=x+y$ also varies. Therefore $B$ alone is not a normalized [hypergeometric distribution](../../../../../../hypergeometric-distribution.md) over $y$; its normalization factor is essential.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
