<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Conditional on $N=n$, the $n$ type indicators are [independent random variables](../../../../../../independent-random-variables.md) with the [Bernoulli distribution](../../../../../../bernoulli-distribution.md) of parameter $p$. Thus $F\mid N=n$ has the [binomial distribution](../../../../../../binomial-distribution.md) and its [probability generating function](../../../../../../probability-generating-function.md) is $(1-p+ps)^n$. The general rule used here is that for a nonnegative integer-valued [random variable](../../../../../../random-variable-split.md) $X$, $G_X(s)=\mathbb E[s^X]$; for a sum of independent such variables, their [probability generating functions](../../../../../../probability-generating-function.md) multiply, since the [expected value](../../../../../../expected-value.md) of the product $s^{X_1}\cdots s^{X_n}$ factors. The [law of total expectation](../../../../../../law-of-total-expectation.md) then averages the conditional result:

$$
G_F(s)=\mathbb E[\mathbb E(s^F\mid N)]=\mathbb E[(1-p+ps)^N]=\boxed{G_N(1-p+ps)},\qquad 0\le s\le1.
$$

This calculation uses the given independent labeling of objects, including conditional on their number.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
