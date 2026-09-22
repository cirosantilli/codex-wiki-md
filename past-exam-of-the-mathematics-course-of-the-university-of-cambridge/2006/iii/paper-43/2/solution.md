<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The claim-size [exponential distribution](../../../../../exponential-distribution.md) has [expected value](../../../../../expected-value.md) $\mu>0$ and [moment-generating function](../../../../../moment-generating-function.md)

$$
M_X(t)=\int_0^\infty e^{tx}\frac1\mu e^{-x/\mu}\,dx=\frac1{1-\mu t},\qquad t<1/\mu.
$$

Conditional on $N_i=k$, [independence](../../../../../independent-random-variables.md) makes the aggregate [moment-generating function](../../../../../moment-generating-function.md) equal to $M_X(t)^k$. Averaging over the [Poisson distribution](../../../../../poisson-distribution.md) of the count gives

$$
\begin{aligned}
M_{S_i}(t)
&=\sum_{k\ge0}e^{-\lambda_i}\frac{\lambda_i^k}{k!}M_X(t)^k\\
&=\exp\big(\lambda_i(M_X(t)-1)\big)
=\boxed{\exp\left(\frac{\lambda_i\mu t}{1-\mu t}\right)}.
\end{aligned}
$$

Put $\Lambda=\sum_{i=1}^n\lambda_i$. For fixed intensities, [independence](../../../../../independent-random-variables.md) between risks gives

$$
M_S(t)=\prod_{i=1}^n M_{S_i}(t)
=\exp\big(\Lambda(M_X(t)-1)\big).
$$

This is precisely the transform of a [compound Poisson distribution](../../../../../compound-poisson-distribution.md). Indeed the [addition of independent Poisson random variables](../../../../../addition-of-independent-poisson-random-variables.md) makes the total count [Poisson distributed](../../../../../poisson-distribution.md) with parameter $\Lambda$, and every claim in the pooled portfolio has the same [exponential distribution](../../../../../exponential-distribution.md). Thus **the portfolio aggregate is compound Poisson with intensity $\sum_i\lambda_i$ and exponential claim sizes of mean $\mu$.**

Now regard the individual intensities as independent [gamma distributed](../../../../../gamma-distribution.md) quantities, with shape $m\ge1$ and rate $\alpha$. Their [moment-generating functions](../../../../../moment-generating-function.md) are $(\alpha/(\alpha-t))^m$ for $t<\alpha$. Multiplying these transforms proves [additivity of independent gamma distributions with a common rate](../../../../../additivity-of-independent-gamma-distributions-with-a-common-rate.md):

$$
\boxed{\Lambda\sim\operatorname{Gamma}(nm,\text{rate }\alpha),\qquad f_\Lambda(\ell)=\frac{\alpha^{nm}}{\Gamma(nm)}\ell^{nm-1}e^{-\alpha\ell},\quad \ell>0.}
$$

Conditional on the individual intensities, the total count $N$ has [Poisson distribution](../../../../../poisson-distribution.md) with parameter $\Lambda$. Because this conditional law depends only on their sum, it is also the law of $N$ conditional on $\Lambda$. Integrating its [probability mass function](../../../../../probability-mass-function.md) against the [gamma distribution](../../../../../gamma-distribution.md) density yields

$$
\begin{aligned}
\mathbb P(N=k)
&=\frac{\alpha^{nm}}{k!\,\Gamma(nm)}\int_0^\infty \ell^{nm+k-1}e^{-(\alpha+1)\ell}\,d\ell\\
&=\frac{\Gamma(nm+k)}{k!\,\Gamma(nm)}\frac{\alpha^{nm}}{(\alpha+1)^{nm+k}}\\
&=\boxed{\binom{nm+k-1}{k}\left(\frac{\alpha}{\alpha+1}\right)^{nm}\left(\frac1{\alpha+1}\right)^k},\qquad k\ge0.
\end{aligned}
$$

Thus **the total count has a [negative binomial distribution](../../../../../negative-binomial-distribution.md) with shape $nm$ and success probability $\alpha/(\alpha+1)$**, using the convention that counts failures before the specified number of successes. Its [probability generating function](../../../../../probability-generating-function.md) is $(\alpha/(\alpha+1-z))^{nm}$.

Conditional on $\Lambda$, the claim sizes retain their common [exponential distribution](../../../../../exponential-distribution.md) and the amount $S$ has a [compound Poisson distribution](../../../../../compound-poisson-distribution.md) of intensity $\Lambda$. Therefore **the unconditional amount has a [compound mixed Poisson distribution](../../../../../compound-mixed-poisson-distribution.md) with gamma mixing intensity of shape $nm$ and rate $\alpha$**. To make the mixture explicit, average the conditional aggregate [moment-generating function](../../../../../moment-generating-function.md):

$$
\begin{aligned}
M_S(t)
&=\mathbb E\exp\big(\Lambda(M_X(t)-1)\big)\\
&=\left(\frac{\alpha}{\alpha-(M_X(t)-1)}\right)^{nm}
=\boxed{\left(\frac{\alpha(1-\mu t)}{\alpha-(\alpha+1)\mu t}\right)^{nm}},
\qquad t<\frac{\alpha}{(\alpha+1)\mu}.
\end{aligned}
$$

The displayed domain ensures both the severity transform and the intensity transform are finite. The mixing distribution describes the Poisson intensity, not the claim sizes. In particular, the aggregate has an atom at zero of mass $\mathbb P(N=0)=(\alpha/(\alpha+1))^{nm}$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
