<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Let $X$ be one score. It has the [discrete uniform distribution](../../../../../discrete-uniform-distribution.md) on $1,\ldots,6$, so its [expected value](../../../../../expected-value.md) and [second moment](../../../../../second-moment.md) are

$$
\mathbb EX=\frac{1+2+3+4+5+6}{6}=\frac72,\qquad
\mathbb EX^2=\frac{1^2+2^2+3^2+4^2+5^2+6^2}{6}=\frac{91}{6}.
$$

Therefore

$$
\boxed{\mathbb EX=\frac72,\qquad\operatorname{Var}(X)=\frac{91}{6}-\frac{49}{4}=\frac{35}{12}.}
$$

For [independent](../../../../../independent-random-variables.md) throws, [linearity of expectation](../../../../../linearity-of-expectation.md) and additivity of [variance](../../../../../variance-split.md) give $\mathbb EY_n=7n/2$ and $\operatorname{Var}(Y_n)=35n/12$. The sample average consequently has [expectation](../../../../../expected-value.md) $7/2$ and [variance](../../../../../variance-split.md) $35/(12n)$.

The [Chebyshev inequality](../../../../../chebyshev-inequality.md) follows by applying the [Markov inequality](../../../../../markov-inequality.md) to the nonnegative square of a centered [random variable](../../../../../random-variable-split.md). It gives

$$
\mathbb P\left(\left|\frac{Y_n}{n}-\frac72\right|>\frac32\right)
\leq\frac{35/(12n)}{(3/2)^2}=\frac{35}{27n}.
$$

This is at most $1/10$ if $n\geq350/27$. Thus **$n=13$ suffices**, as does every larger integer. This is the smallest integer guaranteed by this particular [Chebyshev inequality](../../../../../chebyshev-inequality.md) bound; it need not be the smallest integer satisfying the actual [probability](../../../../../probability.md) requirement.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
