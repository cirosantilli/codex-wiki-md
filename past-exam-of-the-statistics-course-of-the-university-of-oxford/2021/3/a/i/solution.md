<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $S=\sum_i x_i$ and $N=nm$. Conditional [independence](../../../../../independent-random-variables.md) of the [binomial distribution](../../../../../binomial-distribution.md) observations gives the [likelihood function](../../../../../likelihood-function.md)

$$
L(\theta)=\left\{\prod_{i=1}^n\binom m{x_i}\right\}
\theta^S(1-\theta)^{N-S}.
$$

The [prior distribution](../../../../../prior-probability.md) is the [beta distribution](../../../../../beta-distribution.md) with parameters $(1,\beta)$. By [Bayes' theorem](../../../../../bayes-theorem.md), multiplying the [prior density](../../../../../prior-density.md) by the [likelihood function](../../../../../likelihood-function.md) gives a [posterior density](../../../../../posterior-density.md) proportional to

$$
\theta^S(1-\theta)^{N-S+\beta-1}.
$$

Recognizing and normalizing this [beta distribution](../../../../../beta-distribution.md) gives

$$
\boxed{\theta\mid\boldsymbol x\sim\operatorname{Beta}(S+1,N-S+\beta)},\qquad
\boxed{\pi(\theta\mid\boldsymbol x)=
\frac{\theta^S(1-\theta)^{N-S+\beta-1}}{B(S+1,N-S+\beta)}}
$$

for $0<\theta<1$. This is [Beta-binomial conjugacy](../../../../../beta-binomial-conjugacy.md); the original binomial coefficients cancel in the normalization because they are independent of $\theta$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
