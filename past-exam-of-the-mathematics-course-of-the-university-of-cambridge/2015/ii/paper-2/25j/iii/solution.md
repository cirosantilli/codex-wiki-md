<h1 id="25j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $s=\sqrt n/2$. The posterior is $\operatorname{Beta}(X+s,n-X+s)$, and

$$
\boxed{\mathbb E[\theta\mid X]=\frac{X+\sqrt n/2}{n+\sqrt n},\qquad m_{\theta\mid X}=\frac{\max(X+s-1,0)}{\max(X+s,1)+\max(n-X+s,1)-2}.}
$$

The denominator is positive for $n\geq1$. For $n>4$, both parameters exceed one and the mode simplifies to $(X+s-1)/(n+\sqrt n-2)$. For $n=4$ this is the uniform-prior mode, exactly $X/n$; for $n=1,2$ the endpoint or symmetric cases also make the mode rule coincide with $X/n$. Otherwise it is generally a different rule. The [posterior mean](../../../../../../posterior-mean.md) agrees with $X/n$ only at $X=n/2$.

To find the [minimax estimator](../../../../../../minimax-estimator.md) under [quadratic loss](../../../../../../squared-error-loss.md), consider the [posterior mean](../../../../../../posterior-mean.md) $\delta_s=(X+s)/(n+2s)$. Its [risk function](../../../../../../risk-function.md) is

$$
R(\theta,\delta_s)=\frac{n\theta(1-\theta)+s^2(1-2\theta)^2}{(n+2s)^2}.
$$

For $s^2=n/4$, the numerator is identically $n/4$, so

$$
\boxed{R(\theta,\delta_s)=\frac1{4(\sqrt n+1)^2}\quad\text{for all }\theta.}
$$

This [constant-risk binomial proportion estimator](../../../../../../constant-risk-binomial-proportion-estimator.md) is the unique [Bayes estimator](../../../../../../bayes-estimator.md) for its proper beta prior under [quadratic loss](../../../../../../squared-error-loss.md). A competing rule's maximum risk is at least its risk averaged over that prior, which is at least this Bayes risk. The constant-risk rule attains the bound, so **the [posterior mean](../../../../../../posterior-mean.md) in (iii) is the unique minimax rule**. Consequently any coincident rule is minimax too: the mean in (i) is the same rule when $n=4$, and the mean in (ii) is the same rule when $n=1$. No [posterior mode](../../../../../../maximum-a-posteriori-estimate.md) listed here equals that mean rule for every observation, since at $X=0$ its value is positive whereas their endpoint modes differ from it. This accounts for the small-$n$ coincidences as well as the general answer.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [25J](../../25j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
