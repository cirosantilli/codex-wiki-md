# Gumbel distribution

↑ **Parent:** [Extreme value theory](extreme-value-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gumbel_distribution)

The standard [Gumbel distribution](gumbel-distribution.md) for maxima has [distribution function](cumulative-distribution-function.md) $\Lambda(z)=e^{-e^{-z}}$ for every real $z$. Its [probability density function](probability-density-function.md) is the [derivative](derivative.md) of its [distribution function](cumulative-distribution-function.md):

$$
\Lambda(z)=\exp(-e^{-z}),\qquad
g(z)=e^{-z}\exp(-e^{-z}),\qquad z\in\mathbb R.
$$

This article uses the maxima convention throughout. Reflecting a standard [Gumbel distribution](gumbel-distribution.md) [random variable](random-variable-split.md) $Z$ to $-Z$ gives the minima convention, with [distribution function](cumulative-distribution-function.md) $1-\exp(-e^z)$. The two conventions have opposite directions of asymmetry, so their formulas must not be interchanged. [NIST: extreme value type I distributions for maxima and minima](https://www.itl.nist.gov/div898/handbook/eda/section3/eda366g.htm).

For a location $\mu\in\mathbb R$ and positive scale $b>0$, let $Y=\mu+bZ$. This [location-scale family](location-scale-family.md) has [cumulative distribution function](cumulative-distribution-function.md) and [probability density function](probability-density-function.md)

$$
F_Y(x)=\exp\left[-\exp\left(-\frac{x-\mu}{b}\right)\right],\qquad
f_Y(x)=\frac1b\exp\left(-\frac{x-\mu}{b}\right)\exp\left[-\exp\left(-\frac{x-\mu}{b}\right)\right].
$$

Solving $\Lambda(z)=p$ gives the standard [quantile function](quantile-function.md) $q(p)=-\log(-\log p)$, $0<p<1$, and hence the standard [median](median.md)

$$
m=-\log(\log2)\approx0.366513.
$$

The [median](median.md) of $Y$ is therefore $\mu-b\log(\log2)$. Location $\mu$ is not the [median](median.md): at $x=\mu$ the [cumulative distribution function](cumulative-distribution-function.md) is $e^{-1}\approx0.367879$.

To derive the [Gumbel distribution](gumbel-distribution.md) as an extreme-value limit, take the [maximum of independent exponential random variables](maximum-of-independent-exponential-random-variables.md) with rate $\lambda>0$ and set

$$
Z_n=\lambda M_n-\log n.
$$

The exact [distribution function](cumulative-distribution-function.md) is

$$
\mathbb P(Z_n\leq z)=
\begin{cases}
\left(1-\dfrac{e^{-z}}n\right)^n,&z\geq-\log n,\\
0,&z<-\log n.
\end{cases}
$$

The finite-$n$ lower boundary is required because $M_n\geq0$. For each fixed real $z$, eventually $z>-\log n$, and the [natural logarithm](natural-logarithm.md) of the first branch satisfies

$$
n\log\left(1-\frac{e^{-z}}n\right)\longrightarrow-e^{-z}.
$$

Exponentiating proves [convergence in distribution](convergence-in-distribution.md) to the standard [Gumbel distribution](gumbel-distribution.md). It is the familiar [limit](limit-of-a-function.md) $(1-u/n)^n\to e^{-u}$ with $u=e^{-z}$: a simple calculation reveals a whole limiting shape. The name honors Emil Gumbel; Siegrist gives this exponential-maxima derivation and the standard [Gumbel distribution](gumbel-distribution.md) formulas. [Siegrist, Random Services: the Gumbel distribution and its exponential-maxima limit](https://www.randomservices.org/random/special/ExtremeValue.html).

<a id="image-centered-exponential-sample-maxima-for-n-equal-to-1-5-20-and-100-approach-the-standard-gumbel-cumulative-distribution-function"></a>
![](gumbel-limit-exponential-maxima.png)

**[Figure 8](#image-centered-exponential-sample-maxima-for-n-equal-to-1-5-20-and-100-approach-the-standard-gumbel-cumulative-distribution-function). Centered exponential sample maxima for n equal to 1, 5, 20 and 100 approach the standard Gumbel cumulative distribution function**.

For the toy delay model $\lambda=1\,\mathrm{s}^{-1}$, $n=100$, the limiting [Gumbel distribution](gumbel-distribution.md) approximation to $M_{100}$ has $\mu=(\log100)\,\mathrm{s}$ and $b=1\,\mathrm{s}$. Its predicted [median](median.md) is

$$
m_{100}^{\mathrm{approx}}=(\log100-\log(\log2))\,\mathrm{s}\approx4.971683\,\mathrm{s},
$$

compared with the exact [median](median.md) $-\log(1-2^{-1/100})\,\mathrm{s}\approx4.975147\,\mathrm{s}$. The approximation is about $0.003464$ seconds lower in this example. It is not an exact finite-sample [probability distribution](probability-distribution.md): the approximating [Gumbel distribution](gumbel-distribution.md) assigns positive [probability](probability.md) to negative delays, while the exact [sample maximum](sample-maximum.md) cannot be negative.

The [maximum domain of attraction](maximum-domain-of-attraction.md) of the [Gumbel distribution](gumbel-distribution.md) is characterized by an exponential tail ratio on the scale of a [Gumbel auxiliary function](gumbel-auxiliary-function.md). This allows many original [probability distributions](probability-distribution.md) to share the limiting shape, but it does not make the centering $\log n$ appropriate to all of them.

**Table of contents**

- [Moving Gumbel cutoff in an inverse-power tail](moving-gumbel-cutoff-in-an-inverse-power-tail.md)
- [Gumbel limit for gamma maxima](gumbel-limit-for-gamma-maxima.md)
- [Gumbel auxiliary function](gumbel-auxiliary-function.md)

## ↑ Ancestors (6)

1. [Extreme value theory](extreme-value-theory.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Extremal types theorem](extremal-types-theorem.md)
- [Extreme value theory](extreme-value-theory.md)
- [Gumbel distribution](gumbel-distribution.md)
- [Gumbel limit for gamma maxima](gumbel-limit-for-gamma-maxima.md)
- [Max-stable distribution](max-stable-distribution.md)
- [Maximum of independent exponential random variables](maximum-of-independent-exponential-random-variables.md)
- [Moving Gumbel cutoff in an inverse-power tail](moving-gumbel-cutoff-in-an-inverse-power-tail.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/3/solution.md)
- [Return level](return-level.md)
- [Return level plot](return-level-plot.md)
- [Von Mises conditions for extreme values](von-mises-conditions-for-extreme-values.md)
