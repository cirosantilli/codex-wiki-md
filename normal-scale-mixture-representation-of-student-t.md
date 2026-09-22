# Normal scale mixture representation of Student t

↑ **Parent:** [Student's t-distribution](student-s-t-distribution.md)

For [independent](independent-random-variables.md) $Z\sim N(0,1)$ and $\Lambda\sim\chi_\nu^2$, the displayed ratio has the [Student t-distribution](student-s-t-distribution.md) with $\nu>0$ [statistical degrees of freedom](statistical-degrees-of-freedom.md). Equivalently, conditional on $\Lambda=\lambda>0$, $T$ has [normal distribution](normal-distribution.md) $N(0,\nu/\lambda)$. This is a [normal scale mixture representation of Student t](normal-scale-mixture-representation-of-student-t.md): a small latent denominator occasionally produces a much larger spread. The result is a [heavy-tailed distribution](heavy-tailed-distribution.md) even though every conditional [probability distribution](probability-distribution-split.md) is a [normal distribution](normal-distribution.md).

For a short derivation, [independence](independent-random-variables.md) lets us multiply the conditional [normal density](normal-density.md) and the [chi-squared distribution](chi-squared-distribution.md)'s [probability density function](probability-density-function.md), then integrate over the unobserved $\lambda$:

$$
f_\nu(t)=\int_0^\infty \sqrt{\frac{\lambda}{2\pi\nu}}e^{-\lambda t^2/(2\nu)}\frac{\lambda^{\nu/2-1}e^{-\lambda/2}}{2^{\nu/2}\Gamma(\nu/2)}\,d\lambda.
$$

The resulting [gamma function](gamma-function.md) integral has shape $(\nu+1)/2$ and rate $(1+t^2/\nu)/2$, yielding the normalized [probability density function](probability-density-function.md) above. Also, for $\nu>2$, [conditional expectation](conditional-expectation.md) gives $\mathbb E[T^2]=\nu\mathbb E[\Lambda^{-1}]=\nu/(\nu-2)$. Thus unit scale does not mean unit [variance](variance-split.md). Finally, $\mathbb E[\Lambda/\nu]=1$ and $\operatorname{Var}(\Lambda/\nu)=2/\nu$ imply [convergence in probability](convergence-in-probability.md) to 1 by [Chebyshev's inequality](chebyshev-s-inequality.md); [Slutsky's theorem](slutsky-theorem.md) then gives the [standard normal distribution](standard-normal-distribution.md) limit.

## ↑ Ancestors (8)

1. [Student's t-distribution](student-s-t-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Normal scale mixture representation of Student t](normal-scale-mixture-representation-of-student-t.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/3/j/solution.md)
