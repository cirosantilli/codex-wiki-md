<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Insert the shape-two gamma [prior](../../../../../../prior-probability.md) into the integral from part (ii). The [gamma function](../../../../../../gamma-function.md) integral gives

$$
\begin{aligned}
p_n(s)
&=\frac{n^s\lambda^2}{s!}\int_0^\infty\theta^{s+1}e^{-(n+\lambda)\theta}\,d\theta\\
&=\frac{n^s\lambda^2\Gamma(s+2)}{s!(n+\lambda)^{s+2}}\\
&=\boxed{(s+1)\left(\frac\lambda{n+\lambda}\right)^2
\left(\frac n{n+\lambda}\right)^s},\qquad s=0,1,\ldots.
\end{aligned}
$$

Therefore $S_n$ has a [negative binomial distribution](../../../../../../negative-binomial-distribution.md) with shape two and success [probability](../../../../../../probability.md) $\lambda/(n+\lambda)$, using the failures-before-two-successes convention. This is the [Poisson-gamma mixture](../../../../../../poisson-gamma-mixture.md). The identity $\sum_{s\geq0}(s+1)z^s=(1-z)^{-2}$ verifies that the [probabilities](../../../../../../probability.md) sum to one.

Its adjacent [probability](../../../../../../probability.md) ratio is

$$
\frac{p_n(s+1)}{p_n(s)}=\frac{s+2}{s+1}\frac n{n+\lambda}.
$$

Substituting in the [posterior](../../../../../../bayesian-posterior.md) formula gives

$$
\boxed{\mathbb E[X_{n+1}\mid S_n=s]=\frac{s+2}{n+\lambda},}
$$

exactly the estimate from part (i). The equality is required by sufficiency, and the direct computation confirms that the two negative-binomial and gamma parameter conventions have been used consistently.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
