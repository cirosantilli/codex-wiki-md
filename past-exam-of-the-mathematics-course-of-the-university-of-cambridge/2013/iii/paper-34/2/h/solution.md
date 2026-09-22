<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Assuming independent digits under [Benford law](../../../../../../benford-law.md), put $N=\sum_i y_i$ and $p_i=\log_{10}(1+1/i)$. The count vector has a [multinomial distribution](../../../../../../multinomial-distribution.md), with expected counts $E_i=Np_i$. Suitable [predictive discrepancy statistics](../../../../../../predictive-discrepancy-statistic.md) include the [Pearson chi-squared statistic](../../../../../../pearson-chi-squared-statistic.md) and [multinomial deviance](../../../../../../multinomial-deviance.md):

$$
\boxed{T_P=\sum_{i=1}^9\frac{(y_i-E_i)^2}{E_i},\qquad
T_G=2\sum_{i:y_i>0}y_i\log(y_i/E_i).}
$$

The zero-count terms of $T_G$ have limiting value zero. A [Monte Carlo method](../../../../../../monte-carlo-method.md) gives a direct null comparison even when expected counts are small.

For example, an original R implementation is:
```
benford_check <- function(y, B = 9999L) {
  p <- log10(1 + 1/(1:9))
  n <- sum(y)
  expected <- n*p
  observed <- sum((y - expected)^2/expected)
  replicas <- rmultinom(B, size = n, prob = p)
  simulated <- colSums((replicas - expected)^2/expected)
  (1 + sum(simulated >= observed))/(B + 1)
}
```
Each column returned by `rmultinom` is a replicated count vector. R recycles the nine expected counts down each column. The add-one ratio is a [Monte Carlo test](../../../../../../monte-carlo-test.md) estimate. In WinBUGS, alternatively generate a replicated `dmulti` vector using fixed $p_i,N$, compute its discrepancy and monitor exceedance of the observed value. The null does not estimate unknown digit probabilities. Dependence or selection in the accounts would require an appropriate simulation model.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
