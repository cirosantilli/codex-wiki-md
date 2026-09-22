<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A trial of Amy's [rejection sampling](../../../../../rejection-sampling.md) uses exactly $2n$ fair [Bernoulli trials](../../../../../bernoulli-trial.md). Exactly $\binom{2n}{n}$ of the $2^{2n}$ equally likely [binary sequences](../../../../../bitstream.md) have $n$ heads, so the acceptance [probability](../../../../../probability.md) is

$$
p_n=\frac{\binom{2n}{n}}{2^{2n}}.
$$

Independent retries make the number $T$ of trials a [geometric random variable](../../../../../geometric-distribution.md) on $\{1,2,\ldots\}$ with [expectation](../../../../../expected-value-split.md) $1/p_n$. The total number $C$ of coin tosses is $2nT$, so

$$
\boxed{\mathbb EC=\frac{2n\,2^{2n}}{\binom{2n}{n}}.}
$$

Using [Stirling's approximation](../../../../../stirling-formula.md), the [central binomial coefficient](../../../../../central-binomial-coefficient.md) satisfies

$$
\binom{2n}{n}
\sim\frac{\sqrt{4\pi n}(2n/e)^{2n}}{2\pi n(n/e)^{2n}}
=\frac{4^n}{\sqrt{\pi n}}.
$$

Consequently

$$
\boxed{\mathbb EC\sim2\sqrt\pi\,n^{3/2}.}
$$

The [rejection sampling](../../../../../rejection-sampling.md) output is uniform among the balanced [binary sequences](../../../../../bitstream.md): they have equal [probability](../../../../../probability.md) on every trial, and conditioning on acceptance preserves that equality. For $n=0$, the empty output needs zero tosses; the formula above concerns $n\geq1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
