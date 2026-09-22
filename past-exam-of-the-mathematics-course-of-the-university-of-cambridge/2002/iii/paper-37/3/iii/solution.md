<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Using the upper stated [scrapie](../../../../../../scrapie.md)-test-positive fraction, its value among slaughtered sheep is $2000/4000000=0.0005$. The stipulated conditional [BSE](../../../../../../bovine-spongiform-encephalopathy.md) positivity then gives marginal test-positive probability

$$
q=\frac{2000}{4000000}\times0.02=10^{-5},
$$

because the other stratum contributes zero. If the sample consists of independently tested, representative animals, the count $D$ has a [binomial distribution](../../../../../../binomial-distribution.md) with parameters $n,q$. Therefore

$$
\Pr(D=0)=(1-10^{-5})^n\simeq e^{-n10^{-5}}.
$$

The two results are

$$
\boxed{\Pr(D=0\mid n=50000)\simeq0.60653,\qquad
\Pr(D=0\mid n=500000)\simeq0.0067378.}
$$

The [Poisson distribution](../../../../../../poisson-distribution.md) approximation uses mean counts $0.5$ and $5$, respectively. If fewer than 2000 animals belong to the test-positive stratum, these probabilities of finding nothing are higher; the calculation at 2000 is not a guaranteed detection probability.

There is also a sampling-design distinction. If exactly $K$ positive animals in a fixed annual population of $N$ are known and the sample is without replacement, use the [hypergeometric distribution](../../../../../../hypergeometric-distribution.md) instead:

$$
\Pr(D=0)=\frac{\binom{N-K}{n}}{\binom Nn}.
$$

The given expected prevalence does not assert an exactly fixed $K$, so the independent prevalence model is the natural interpretation of the requested calculation.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
