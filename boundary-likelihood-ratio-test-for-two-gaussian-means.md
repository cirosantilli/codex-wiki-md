# Boundary likelihood-ratio test for two Gaussian means

↑ **Parent:** [Likelihood-ratio test](likelihood-ratio-test.md)

For independent unit-variance Gaussian samples with means $\mu_X,\mu_Y$, testing $\mu_X\geq A,\mu_Y=0$ against unrestricted means gives $T=-2\log\Lambda=n[\bar Y^2+(A-\bar X)_+^2]$. The unrestricted [maximum-likelihood estimators](maximum-likelihood-estimator.md) are the two [sample means](sample-mean.md), while the null estimators are $\max(A,\bar X)$ and zero. Under the null, write $W=\sqrt n(\bar X-A)=W_0+\delta$, $\delta=\sqrt n(\mu_X-A)\geq0$, and $Z=\sqrt n\bar Y$, with $W_0,Z$ independent standard Gaussian variables. Then $T=Z^2+(-W_0-\delta)_+^2$ decreases pointwise with $\delta$, so the largest rejection probability occurs at the boundary $\mu_X=A$. There its law is the [chi-bar-squared distribution](chi-bar-squared-distribution.md) $\tfrac12\chi_1^2+\tfrac12\chi_2^2$. The exact size-$\alpha$ threshold $c_\alpha$ is therefore determined by $1-\Phi(\sqrt{c_\alpha})+\tfrac12e^{-c_\alpha/2}=\alpha$.

## ↑ Ancestors (8)

1. [Likelihood-ratio test](likelihood-ratio-test.md)
2. [Statistical hypothesis test](statistical-hypothesis-test.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
