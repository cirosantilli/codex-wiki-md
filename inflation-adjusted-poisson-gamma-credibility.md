# Inflation-adjusted Poisson-gamma credibility

↑ **Parent:** [Bayesian credibility](bayesian-credibility.md)

For a common [gamma distribution](gamma-distribution.md) (shape $\alpha$, rate $\beta$) frequency [prior distribution](prior-probability.md) and conditionally [independent](independent-random-variables.md) [Poisson distribution](poisson-distribution.md) yearly counts of means $w_j\Theta$, observed average amounts $y_j$ determine counts $k_j=w_jy_j/c_j$. The [posterior distribution](bayesian-posterior.md) shape is $\alpha+\sum_jk_j$ and rate is $\beta+\sum_jw_j$. The future per-policy [mean](expected-value.md) is the display, equal to [credibility factor](credibility-factor.md) $W/(W+\beta)$ times $\sum_j(w_j/W)(c_{n+1}/c_j)y_j$ plus the complementary weight times $c_{n+1}\alpha/\beta$. The data must lie on their count lattice; impossible noninteger recovered counts have zero [likelihood](likelihood-function.md).

// Destination: probability-theory.bigb

## ↑ Ancestors (7)

1. [Bayesian credibility](bayesian-credibility.md)
2. [Credibility estimate](credibility-estimate.md)
3. [Actuarial statistics](actuarial-statistics-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-41/4/solution.md)
