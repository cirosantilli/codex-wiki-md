# Power law

↑ **Parent:** [Analysis](analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Power_law)

A [power law](power-law.md) is a relation $f(x)=Cx^p$, with fixed constants $C$ and $p$. For positive $x$, any [real number](real-number.md) $p$ is allowed. Its useful feature is a simple scaling rule:

$$
f(\lambda x)=\lambda^p f(x)\qquad(\lambda>0).
$$

The same proportional change of input produces the same proportional change of output, independently of the starting value. The exponent controls that response; the coefficient fixes the magnitude.

For example, the [area](surface-area.md) of a [circle](circle.md) is $A(r)=\pi r^2$. Doubling the [radius](radius.md) multiplies its [area](surface-area.md) by four, and tripling it multiplies the [area](surface-area.md) by nine. The [volume](volume.md) of a [sphere](sphere.md) is $V(r)=4\pi r^3/3$: the same changes multiply its [volume](volume.md) by eight and twenty-seven. The distinction explains why similarly shaped objects do not preserve their ratio of [surface area](surface-area.md) to [volume](volume.md) when their size changes.

When the output is positive, a [logarithm](logarithm.md) turns the [power law](power-law.md) into a straight-line relation. Using positive reference values $x_0$ and $f_0=f(x_0)$,

$$
\frac{f(x)}{f_0}=\left(\frac{x}{x_0}\right)^p,
\qquad
\log\frac{f(x)}{f_0}=p\log\frac{x}{x_0}.
$$

These ratios are [dimensionless quantities](dimensionless-quantity.md), so the formula also applies to physical measurements with units. Plotting both ratios on a [logarithmic scale](logarithmic-scale.md) gives a line of slope $p$. Changing a unit changes the numerical coefficient, while the exponent stays the same. Positive $p$ describes increasing values; negative $p$ describes decreasing values; $p=0$ gives a constant. The zero coefficient is a degenerate case with no useful logarithmic slope.

Exact scaling is stronger than [regular variation](regular-variation.md). The [function](function-split.md) $x^2\log x$ has a doubling ratio tending to four, but its logarithmic correction keeps growing. The diagram contrasts it with the exact [power law](power-law.md) $x^2$.

<a id="image-exact-quadratic-scaling-and-a-logarithmic-correction-have-different-finite-doubling-ratios-even-though-the-correction-leaves-the-limiting-exponent-unchanged"></a>
![](regular-variation-rescaling-ratios.png)

**[Figure 1](#image-exact-quadratic-scaling-and-a-logarithmic-correction-have-different-finite-doubling-ratios-even-though-the-correction-leaves-the-limiting-exponent-unchanged). Exact quadratic scaling and a logarithmic correction have different finite doubling ratios, even though the correction leaves the limiting exponent unchanged**.

A [power law](power-law.md) for a [probability density](probability-density.md) and a [power law](power-law.md) for a [tail probability](tail-probability.md) have different exponents. For a [Pareto distribution](pareto-distribution.md) with $\alpha>0$ and lower endpoint one,

$$
\mathbb P(X>x)=x^{-\alpha},
\qquad
p_X(x)=\alpha x^{-\alpha-1}
\qquad(x>1).
$$

The [tail probability](tail-probability.md) has exponent $-\alpha$; differentiating it and changing sign gives the [probability density](probability-density.md) exponent $-\alpha-1$. Confusing them changes the interpretation of a fitted exponent. The normalizing coefficient and lower endpoint also matter: a decreasing [power law](power-law.md) is not automatically a valid [probability density](probability-density.md) over the entire positive [real line](real-line.md).

The appearance of a line over a finite logarithmic range is evidence to investigate, rather than a proof of an exact [power law](power-law.md) or its mechanism. In their study of [power-law distributions](power-law-distribution.md), Clauset, Shalizi and Newman combine [maximum likelihood estimation](maximum-likelihood-estimation.md), [goodness-of-fit tests](goodness-of-fit-test.md) and comparisons with alternative models; their abstract explains why ordinary least-squares fitting can give misleading results for tail data. See [Aaron Clauset, Cosma Rohilla Shalizi and M. E. J. Newman, Power-law distributions in empirical data, SIAM Review 51 (2009), 661–703](https://arxiv.org/abs/0706.1062). The scaling rule is mathematically exact when it defines a model; whether a dataset supports that model is a question of [statistical inference](statistical-inference-split.md).

**Table of contents**

- [Power-law distribution](power-law-distribution.md)
- [Cored power-law density profile](cored-power-law-density-profile.md)
- [Polynomial growth](polynomial-growth.md)

## ↑ Ancestors (4)

1. [Analysis](analysis-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (34)

- [Cored power-law density profile](cored-power-law-density-profile.md)
- [Galaxy-conditioned neighbour count](galaxy-conditioned-neighbour-count.md)
- [Kepler's third law](kepler-s-third-law.md)
- [Linear low-temperature heat capacity of a two-dimensional Fermi gas](linear-low-temperature-heat-capacity-of-a-two-dimensional-fermi-gas.md)
- [Mass-spectrum transport under quadratic accretion](mass-spectrum-transport-under-quadratic-accretion.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-41/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-41/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-67/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-67/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-51/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-83/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-83/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-89/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-90/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/15e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-61/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-63/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-317/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/35d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-349/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-346/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-332/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-344/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-349/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-352/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-310/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-346/4/solution.md)
- [Power law](power-law.md)
- [Power-law distribution](power-law-distribution.md)
- [Regular variation](regular-variation.md)
- [Sea-ice lead-width distribution](sea-ice-lead-width-distribution.md)
- [Self-gravitating Kramers power-law envelope](self-gravitating-kramers-power-law-envelope.md)
- [Slowly varying function](slowly-varying-function.md)
