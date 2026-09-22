# Laplace prior for sparse images

↑ **Parent:** [Laplace distribution](laplace-distribution.md)

Independent centered [Laplace distributions](laplace-distribution.md) for pixel intensities give the [prior distribution](prior-probability.md)

$$
\pi_0(u)=(\lambda/2)^d e^{-\lambda\sum_{j=1}^d|u_j|},\qquad\lambda>0.
$$

This prior favors small intensities through its sharp peak at zero, while its tails permit isolated appreciable pixels. Its negative log density is an [L1 norm](l1-norm.md) penalty, so with a [Gaussian likelihood](gaussian-likelihood.md) a [maximum a posteriori estimate](maximum-a-posteriori-estimate.md) minimizes a sum of squared residuals plus that penalty. A draw from this continuous prior has no exactly zero coordinate with positive probability; sparsity of a maximizing estimate and concentration of prior mass near zero are different statements. The product prior also does not encode spatial contiguity. [Inverse transform sampling](inverse-transform-sampling.md) produces each coordinate from an independent [uniform distribution](continuous-uniform-distribution.md) by $\lambda^{-1}\log(2U)$ for $U\leq1/2$ and $-\lambda^{-1}\log(2(1-U))$ otherwise, ignoring the probability-zero endpoints.

## ↑ Ancestors (8)

1. [Laplace distribution](laplace-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/2/b/solution.md)
