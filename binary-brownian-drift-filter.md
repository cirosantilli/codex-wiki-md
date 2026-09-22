# Binary Brownian drift filter

↑ **Parent:** [Innovation process](innovation-process.md)

For $X_t=W_t+\alpha t$ with an independent equiprobable drift $\alpha\in\{-a,a\}$, the [likelihood ratio](likelihood-ratio.md) between the two drifts is $e^{2aX_t}$. Multiplying the [normal distribution](normal-distribution.md) densities of successive increments proves this ratio for every observation partition; continuity then gives the full observed-path posterior. The [Bayes' theorem](bayes-theorem.md) gives $q_t=\mathbb P(\alpha=a\mid\mathcal F_t^X)=(1+e^{-2aX_t})^{-1}$. Thus the observed drift is $a(2q_t-1)=a\tanh(aX_t)$. The process $\widehat W_t=X_t-\int_0^t a\tanh(aX_s)ds$ is an observed-filtration [martingale](martingale-split.md) with [quadratic variation](quadratic-variation.md) $t$, so the [Lévy characterization of Brownian motion](levy-characterization-of-brownian-motion.md) makes it a [Brownian motion](brownian-motion-split.md). The observed state is a scaled [diffusion with hyperbolic tangent drift](diffusion-with-hyperbolic-tangent-drift.md).

## ↑ Ancestors (6)

1. [Innovation process](innovation-process.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Learning hedge in a binary-drift investment model](learning-hedge-in-a-binary-drift-investment-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39/4/ii/solution.md)
