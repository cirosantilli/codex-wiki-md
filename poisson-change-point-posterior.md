# Poisson change-point posterior

↑ **Parent:** [Change-point detection](change-point-detection.md)

For an [Inhomogeneous Poisson process](inhomogeneous-poisson-process.md) whose known positive intensity changes from $\lambda_1$ to $\lambda_2$ at an unknown time $\theta\in(0,T)$, the ordered arrival-time [likelihood function](likelihood-function.md) is

$$
L(\theta)=\lambda_1^{j(\theta)}\lambda_2^{n-j(\theta)}e^{-\lambda_1\theta-\lambda_2(T-\theta)}.
$$

Under a [uniform prior](uniform-prior.md), each interval between successive arrivals has an exponential [posterior density](posterior-density.md) with rate in the exponent $\lambda_2-\lambda_1$. Its integrated weights allow exact interval selection followed by a truncated exponential draw; when the two rates coincide, the [Bayesian posterior](bayesian-posterior.md) is uniform and the data contain no change-time information.

## ↑ Ancestors (5)

1. [Change-point detection](change-point-detection.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/1/h/solution.md)
- [Poisson count change-point model with gamma priors](poisson-count-change-point-model-with-gamma-priors.md)
