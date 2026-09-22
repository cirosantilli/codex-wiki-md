# EM update for a single-factor Gaussian model

↑ **Parent:** [Factor analysis](factor-analysis.md)

In [factor analysis](factor-analysis.md) with one factor and fixed noise variance $v>0$, let $\lambda$ be the current loading vector, $s=v+|\lambda|^2$, and $S=n^{-1}\sum_iY_iY_i^T$. The [expectation-maximization algorithm](expectation-maximization-algorithm.md) update is

$$
\lambda_{\mathrm{new}}=\frac{sS\lambda}{vs+\lambda^TS\lambda}.
$$

The conditional factor means are $\lambda^TY_i/s$ and their variances are $v/s$; maximizing the expected complete-data log-likelihood gives the formula.

## ↑ Ancestors (8)

1. [Factor analysis](factor-analysis.md)
2. [Latent variable](latent-variable.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/4/b/solution.md)
