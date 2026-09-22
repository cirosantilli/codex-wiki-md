# Ordered-rate exponential M-step

↑ **Parent:** [Expectation-maximization algorithm](expectation-maximization-algorithm.md)

For $N$ observations from each of two labeled [exponential distributions](exponential-distribution.md), an E-step may produce positive completed time totals $U,V$. Its expected complete-data [log-likelihood](log-likelihood.md) is $Q=N\log\lambda_1+N\log\lambda_2-U\lambda_1-V\lambda_2$. This is strictly [concave](concave-function.md). On the closed ordering constraint $\lambda_1\geq\lambda_2>0$, its maximum is $(N/U,N/V)$ when $U<V$; otherwise it lies at $\lambda_1=\lambda_2=2N/(U+V)$. To see the boundary case, first maximize along the equality line. At that maximum, moving into either feasible rate-separating direction has directional [derivative](derivative.md) $(V-U)/2\leq0$, so [concavity](concave-function.md) proves global optimality. For the open constraint $\lambda_1>\lambda_2$, this boundary value is a supremum rather than an attained M-step.

// Target: probability-and-statistics.bigb

## ↑ Ancestors (8)

1. [Expectation-maximization algorithm](expectation-maximization-algorithm.md)
2. [Latent variable](latent-variable.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/5/c/solution.md)
