# Uniformly most powerful test for a gamma rate

↑ **Parent:** [Neyman-Pearson lemma](neyman-pearson-lemma.md)

For an independent [statistical sample](statistical-sample.md) from a [gamma distribution](gamma-distribution.md) with known shape $\lambda>0$ and unknown rate $\theta>0$, test $\theta=\theta_0$ against $\theta>\theta_0$. The alternative-to-null [likelihood ratio](likelihood-ratio.md) for any larger rate $\theta_1$ is $(\theta_1/\theta_0)^{n\lambda}\exp\{-(\theta_1-\theta_0)S\}$, where $S=\sum_iX_i$. This decreases in $S$, so the [Neyman-Pearson lemma](neyman-pearson-lemma.md) gives one common lower-tail ordering for all alternatives.

Let $G_a$ be the unit-rate [gamma distribution](gamma-distribution.md) [cumulative distribution function](cumulative-distribution-function.md) with shape $a$. The [uniformly most powerful test](uniformly-most-powerful-test.md) of exact [test size](size-of-a-statistical-test.md) $\alpha\in(0,1)$ rejects when $S<c_\alpha$, where $c_\alpha=G_{n\lambda}^{-1}(\alpha)/\theta_0$. Its [power function](power-function-of-a-statistical-test.md) is displayed above. If $n\lambda=1$, the sum has an [exponential distribution](exponential-distribution.md), so $c_\alpha=-\log(1-\alpha)/\theta_0$ and $\pi(\theta)=1-(1-\alpha)^{\theta/\theta_0}$. Monotonicity of $G_a(\theta c_\alpha)$ also makes this test valid and uniformly most powerful for the larger [null hypothesis](null-hypothesis.md) $\theta\leq\theta_0$.

## ↑ Ancestors (8)

1. [Neyman-Pearson lemma](neyman-pearson-lemma.md)
2. [Statistical hypothesis test](statistical-hypothesis-test-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2021/2/c/solution.md)
