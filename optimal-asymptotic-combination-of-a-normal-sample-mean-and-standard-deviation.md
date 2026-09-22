# Optimal asymptotic combination of a normal sample mean and standard deviation

↑ **Parent:** [Normal sample](normal-sample.md)

In the [normal mean proportional to standard deviation model](normal-mean-proportional-to-standard-deviation-model.md), both $\overline X$ and $S$ estimate the positive [statistical parameter](statistical-parameter.md) $\mu$. Their independent limiting [normal distributions](normal-distribution.md) have rescaled [variances](variance-split.md) $\mu^2$ and $\mu^2/2$, respectively, by [asymptotic normality of a normal sample standard deviation](asymptotic-normality-of-a-normal-sample-standard-deviation.md). Thus for fixed $w\in\mathbb R$,

$$
\sqrt n\{w\overline X+(1-w)S-\mu\}\xrightarrow dN\!\left(0,\mu^2\left[w^2+\frac{(1-w)^2}{2}\right]\right).
$$

The bracket is $3(w-1/3)^2/2+1/3$, minimized uniquely at $w=1/3$. Hence $(\overline X+2S)/3$ has leading sampling [variance](variance-split.md) $\mu^2/(3n)$, the inverse expected [Fisher information](fisher-information-matrix.md). The result is first-order optimality within these fixed-weight combinations and does not assert that $S$ is an exactly [unbiased estimator](unbiased-estimator.md).

## ↑ Ancestors (7)

1. [Normal sample](normal-sample.md)
2. [Statistical sample](statistical-sample.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Normal mean proportional to standard deviation model](normal-mean-proportional-to-standard-deviation-model.md)
- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2017/1/b/iii/solution.md)
