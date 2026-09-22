<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Given $\Theta=\theta$, the sum of the independent yearly counts is $S_n\sim\operatorname{Poisson}(n\theta)$: their [probability generating functions](../../../../../../probability-generating-function.md) multiply to $\exp(n\theta(z-1))$. Averaging this conditional law over the [prior](../../../../../../prior-probability.md) gives the [mixed Poisson distribution](../../../../../../mixed-poisson-distribution.md)

$$
\boxed{p_n(s):=\mathbb P(S_n=s)
=\frac{n^s}{s!}\int_0^\infty e^{-n\theta}\theta^s\pi(\theta)\,d\theta,\qquad s\geq0.}
$$

The likelihood for the full vector depends on $\theta$ only through $s$, so $S_n$ is a [sufficient statistic](../../../../../../sufficient-statistic.md); conditioning on the total or on the full observed vector gives the same [posterior](../../../../../../bayesian-posterior.md) for $\Theta$.

For an event of positive [probability](../../../../../../probability.md) $p_n(s)>0$, the [posterior density](../../../../../../posterior-density.md) is proportional to $e^{-n\theta}\theta^s\pi(\theta)$. Put $I_s=\int_0^\infty e^{-n\theta}\theta^s\pi(\theta)\,d\theta$. Its mean is $I_{s+1}/I_s$. The future count has [conditional mean](../../../../../../conditional-expectation.md) $\Theta$, so

$$
\begin{aligned}
\mathbb E[X_{n+1}\mid S_n=s]
&=\frac{I_{s+1}}{I_s}\\
&=\frac{(s+1)!\,p_n(s+1)/n^{s+1}}{s!\,p_n(s)/n^s}
=\boxed{\frac{(s+1)\mathbb P(S_n=s+1)}{n\mathbb P(S_n=s)}}.
\end{aligned}
$$

This is the [posterior mean from adjacent mixed Poisson probabilities](../../../../../../posterior-mean-from-adjacent-mixed-poisson-probabilities.md). Both [probabilities](../../../../../../probability.md) refer to the same $n$-year exposure; the numerator is not a [probability](../../../../../../probability.md) for $S_{n+1}$. For a proper [prior](../../../../../../prior-probability.md) and $n>0$, the integrals defining this [posterior mean](../../../../../../posterior-mean.md) are finite because $\theta^{s+1}e^{-n\theta}$ is bounded on $[0,\infty)$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
