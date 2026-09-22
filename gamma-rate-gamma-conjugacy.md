# Gamma rate gamma conjugacy

↑ **Parent:** [Conjugate prior](conjugate-prior.md)

Conditionally independent [gamma distributions](gamma-distribution.md) with known shape $r$ and unknown rate $\Theta$ have likelihood proportional to $\Theta^{nr}e^{-\Theta\sum_i x_i}$. A [gamma distribution](gamma-distribution.md) prior of shape $A$ and rate $B$ therefore updates to shape $A+nr$ and rate $B+\sum_i x_i$. When $A+nr>1$, the [posterior mean](posterior-mean.md) of the conditional claim mean $r/\Theta$ is $r(B+\sum_i x_i)/(A+nr-1)$. For $A=rk+1$ and $B=k\mu$, this is a [credibility estimate](credibility-estimate.md) with weight $n/(n+k)$. It is the reciprocal-rate version of [gamma scale inverse-gamma conjugacy](gamma-scale-inverse-gamma-conjugacy.md).

## ↑ Ancestors (8)

1. [Conjugate prior](conjugate-prior.md)
2. [Exponential family](exponential-family-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-40/4/solution.md)
