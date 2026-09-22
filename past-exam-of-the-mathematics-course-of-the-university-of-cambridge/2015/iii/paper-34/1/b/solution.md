<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To distinguish the random intensity from its possible values, write it as $\Lambda$. Its law is a [gamma distribution](../../../../../../gamma-distribution.md) with shape $2$ and rate $p/q$. Hence

$$
\boxed{\lambda_0=\mathbb E\Lambda=\frac{2q}{p}},\qquad
\operatorname{Var}(\Lambda)=\frac{2q^2}{p^2}.
$$

For the [Poisson mixture](../../../../../../poisson-mixture.md), [conditional expectation](../../../../../../conditional-expectation.md) and [conditional variance](../../../../../../conditional-variance.md) both equal $\Lambda$. The [law of total expectation](../../../../../../law-of-total-expectation.md) and the [law of total variance](../../../../../../law-of-total-variance.md) yield

$$
\mathbb EN=\frac{2q}{p},\qquad
\operatorname{Var}(N)=\mathbb E\Lambda+\operatorname{Var}(\Lambda)
=\frac{2q}{p^2},
$$

where $p+q=1$. Applying the [random sum of independent claims](../../../../../../random-sum-of-independent-claims.md) formulas with the [exponential distribution](../../../../../../exponential-distribution.md) of the claim sizes gives **the portfolio B moments**

$$
\boxed{\mathbb ES_B=\frac{2q\mu}{p},\qquad
\operatorname{Var}(S_B)=\frac{2q(1+p)\mu^2}{p^2}.}
$$

At the matched intensity $\lambda_0$, the [expected value](../../../../../../expected-value.md) for portfolio A is also $2q\mu/p$, whereas its [variance](../../../../../../variance-split.md) is $4q\mu^2/p$. Thus **the expected totals agree, but mixing increases the variance**:

$$
\boxed{\operatorname{Var}(S_B)-\operatorname{Var}(S_A)
=\frac{2q^2\mu^2}{p^2}>0.}
$$

The extra term is precisely $\mu^2\operatorname{Var}(\Lambda)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
