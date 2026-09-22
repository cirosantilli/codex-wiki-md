# EM for zero-inflated negative binomial regression

↑ **Parent:** [Zero-inflated negative binomial model](zero-inflated-negative-binomial-model.md)

For known size $r$ and $\lambda_i=e^{x_i^T\beta}$, the [expectation-maximization algorithm](expectation-maximization-algorithm.md) gives structural-zero responsibility $t_i=0$ for positive counts and $t_i=\pi/[\pi+(1-\pi)(r/(r+\lambda_i))^r]$ for zero counts. This is [Bayes' theorem](bayes-theorem.md). Maximizing the expected complete-data [log-likelihood](log-likelihood.md) gives $\pi_{\rm new}=n^{-1}\sum_i t_i$ and a weighted [negative binomial regression](negative-binomial-regression.md) with weights $1-t_i$. The objective separates into a Bernoulli mixing term and a weighted count term, which proves the update.

## ↑ Ancestors (8)

1. [Zero-inflated negative binomial model](zero-inflated-negative-binomial-model.md)
2. [Zero inflation](zero-inflation.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/1/f/solution.md)
