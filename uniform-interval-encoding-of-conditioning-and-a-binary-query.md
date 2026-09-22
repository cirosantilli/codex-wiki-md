# Uniform-interval encoding of conditioning and a binary query

↑ **Parent:** [Probabilistic program](probabilistic-program.md)

Let a model have parameter [prior density](prior-density.md) $\rho$, observation [probability](probability.md) $L(\theta)\in[0,1]$ and conditional binary-query [probability](probability.md) $h(\theta)\in[0,1]$ after observation. Draw $\theta\sim\rho$ and an independent [uniform random variable](uniform-random-variable.md) $U$. Accept exactly when $U<L(\theta)$, then output whether $U<L(\theta)h(\theta)$. At fixed $\theta$, the accepted true and false intervals have lengths $Lh$ and $L(1-h)$. Integrating against $\rho$ and dividing by the positive evidence proves equality of the joint posterior law of parameters and answer. This can replace many latent choices by one auxiliary coordinate. It preserves that joint law, not unreported latent traces. More generally the bounded factor must be a [probability](probability.md) or first be divided by a valid common rejection envelope.

## ↑ Ancestors (5)

1. [Probabilistic program](probabilistic-program.md)
2. [Probabilistic programming](probabilistic-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/3/c/solution.md)
