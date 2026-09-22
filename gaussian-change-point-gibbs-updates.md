# Gaussian change-point Gibbs updates

↑ **Parent:** [Gaussian change-point posterior with proper priors](gaussian-change-point-posterior-with-proper-priors.md)

For independent means $\theta\sim N(\mu_\theta,t_\theta)$ and $\phi\sim N(\mu_\phi,t_\phi)$, the first mean's conditional precision is $m/v+1/t_\theta$ and conditional precision-weighted mean is $\sum_{i\le m}x_i/v+\mu_\theta/t_\theta$; replace $m$ by $n-m$ for the second mean. With $v\sim\operatorname{IG}(a_0,b_0)$ its conditional law is $\operatorname{IG}(a_0+n/2,b_0+S_m/2)$. The discrete split has conditional probabilities proportional to $e^{-S_m/(2v)}$. These [full conditional distributions](full-conditional-distribution.md) give a [Gibbs sampler](gibbs-sampler.md) including $m=n$. Averaging the sampled indicators of that configuration estimates its [probability](probability.md); averaging its conditional probabilities gives an estimate by [Rao-Blackwellization](rao-blackwellization.md).

## ↑ Ancestors (6)

1. [Gaussian change-point posterior with proper priors](gaussian-change-point-posterior-with-proper-priors.md)
2. [Change-point detection](change-point-detection.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/5/solution.md)
