# Fisher information loss from thresholding an exponential observation

↑ **Parent:** [Fisher information matrix](fisher-information-matrix.md)

If $X$ has an [exponential distribution](exponential-distribution.md) with rate $\lambda>0$, a full observation has [Fisher information](fisher-information-matrix.md) $1/\lambda^2$. Recording only $Y=\mathbf1_{\{X>T\}}$ for a fixed $T>0$ instead gives a [Bernoulli distribution](bernoulli-distribution.md) with parameter $r=e^{-\lambda T}$. The chain rule for its [score function](informant-function.md) gives

$$
I_Y(\lambda)=\frac{(r')^2}{r(1-r)}=\frac{T^2}{e^{\lambda T}-1},\qquad
\frac{I_Y}{I_X}=\frac{s^2}{e^s-1}<1,\quad s=\lambda T.
$$

To see the strict inequality, write $e^s-1=s+s^2/2+s^3/6+\cdots$. For $0<s\le1$ the first two terms already exceed $s^2$. For $s\ge1$, the function $e^s-1-s^2$ is positive at one, its derivative $e^s-2s$ is positive there, and that derivative is increasing for $s\ge1$. Thus every positive threshold discards information. For independent observations, both information quantities multiply by the sample size. The [Cramér-Rao bound](cramer-rao-bound.md) and [asymptotic normality of a maximum likelihood estimator](asymptotic-normality-of-a-maximum-likelihood-estimator.md) explain the corresponding loss of attainable precision.

## ↑ Ancestors (8)

1. [Fisher information matrix](fisher-information-matrix.md)
2. [Informant function](informant-function.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
