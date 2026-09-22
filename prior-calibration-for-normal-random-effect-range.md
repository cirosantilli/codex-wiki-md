# Prior calibration for normal random-effect range

↑ **Parent:** [Between-study heterogeneity](between-study-heterogeneity.md)

For $J\ge2$ conditionally independent effects $\beta_j\sim N(\mu,\tau^2)$, each pair difference has [normal distribution](normal-distribution.md) $N(0,2\tau^2)$. With $m=\binom J2$, an upper bound $A=R/[\sqrt2\,\Phi^{-1}(1-\varepsilon/(2m))]$ on $\tau$ ensures, by the [union bound](boole-s-inequality.md), that $\mathbb P(\max_j\beta_j-\min_j\beta_j>R)\le\varepsilon$. Any proper scale [prior distribution](prior-probability.md) supported on $(0,A)$ preserves this bound after averaging. This is conservative simultaneous calibration, rather than the weaker statement about one selected pair. For [log odds ratios](log-odds-ratio.md), a bound $R$ corresponds to a ratio-of-odds-ratios bound $e^R$.

## ↑ Ancestors (8)

1. [Between-study heterogeneity](between-study-heterogeneity.md)
2. [Random-effects meta-analysis](random-effects-meta-analysis.md)
3. [Meta-analysis](meta-analysis.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/4/e/solution.md)
