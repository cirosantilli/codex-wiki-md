# Simultaneous empirical distribution confidence band

↑ **Parent:** [Empirical distribution function](empirical-distribution-function.md)

Fix a failure [probability](probability.md) $0<\alpha<1$ and assume an [independent and identically distributed](independent-and-identically-distributed-random-variables.md) [statistical sample](statistical-sample.md). A finite-sample [confidence band](confidence-band.md) for its population [cumulative distribution function](cumulative-distribution-function.md) is

$$
\varepsilon_{n,\alpha}=\sqrt{\frac{\log(2/\alpha)}{2n}},\qquad
L_n(x)=\max\{0,F_n(x)-\varepsilon_{n,\alpha}\},\qquad
U_n(x)=\min\{1,F_n(x)+\varepsilon_{n,\alpha}\}.
$$

Here $\log$ is the [natural logarithm](natural-logarithm.md). The [DKW inequality](dvoretzky-kiefer-wolfowitz-inequality.md) implies

$$
\mathbb P\!\left(L_n(x)\leq F(x)\leq U_n(x)\text{ for every }x\in\mathbb R\right)\geq1-\alpha.
$$

This is simultaneous coverage over the whole [real line](real-line.md), valid at each fixed sample size.[§2.1, printed p. 15, Theorem 2.6 and the derivation preceding it](all-of-nonparametric-statistics-by-larry-wasserman.md)

To obtain the band, solve $2e^{-2n\varepsilon^2}=\alpha$ for the positive $\varepsilon$. Outside a failure [event](event.md) of [probability](probability.md) at most $\alpha$, $|F_n(x)-F(x)|\leq\varepsilon_{n,\alpha}$ for every $x$. Since a [cumulative distribution function](cumulative-distribution-function.md) already lies in $[0,1]$, clipping the endpoints to this [interval](interval-mathematics.md) preserves the coverage [event](event.md). The guarantee is at least $1-\alpha$, and need not equal it.

Choose $\alpha=0.1$, giving at least $90\%$ simultaneous coverage under the stated model. For $n=5,50,500$, respectively, the half-widths before clipping are

$$
\varepsilon_{5,0.1}\approx0.54733,\qquad
\varepsilon_{50,0.1}\approx0.17308,\qquad
\varepsilon_{500,0.1}\approx0.054733.
$$

For the chosen five observations, the band at $x=1$ is $[0,0.94733]$, while at $x=4$ it is approximately $[0.25267,1]$. At $x=3$ the unclipped band would be $[0.05267,1.14733]$, so clipping gives $[0.05267,1]$. The broad uncertainty is informative: five observations give a precise description of themselves, but a coarse bound for an unknown population [cumulative distribution function](cumulative-distribution-function.md).

<a id="image-finite-sample-simultaneous-uncertainty-around-an-empirical-distribution-function"></a>
![](empirical-distribution-simultaneous-uncertainty.png)

**[Figure 7](#image-finite-sample-simultaneous-uncertainty-around-an-empirical-distribution-function). Finite-sample simultaneous uncertainty around an empirical distribution function**. Left: the chosen five observations give $F_5$ and its band clipped to $[0,1]$, using $\alpha=0.1$. Right: theoretical half-widths for $n=5,50,500$, with no additional samples constructed. The [confidence band](confidence-band.md) has coverage at least $90\%$ under [independent and identically distributed](independent-and-identically-distributed-random-variables.md) sampling; the drawing illustrates the procedure and does not establish its coverage.

A collection of $90\%$ pointwise [confidence intervals](confidence-interval.md) only promises coverage separately at each preselected threshold; it does not promise $90\%$ coverage of an entire [cumulative distribution function](cumulative-distribution-function.md). Here the one simultaneous [event](event.md) permits inspecting any threshold after seeing the data. The [probability](probability.md) refers to repeated sampling of the entire [statistical sample](statistical-sample.md), with $F$ fixed. It does not assign $90\%$ [probability](probability.md) to a fixed $F$ after observing this particular band, and it is not a [prediction interval](prediction-interval.md) for a future observation. The displayed $n=5,50,500$ comparison gives a guarantee for each fixed $n$ separately, not simultaneous validity over all sample sizes or an optional stopping rule. The chosen observations are an illustration; the coverage claim follows from the [DKW inequality](dvoretzky-kiefer-wolfowitz-inequality.md), not from their appearance or a simulation. Dependence or observations with different sampling laws require another argument.

At fixed $\alpha$, multiplying $n$ by $100$ divides the half-width by $10$. Conversely, a desired half-width $\delta>0$ is ensured by $n\geq\log(2/\alpha)/(2\delta^2)$, rounded up to an [integer](integer-split.md). For $\alpha=0.1$ and $\delta=0.1$, this sufficient sample size is $150$. This makes the [confidence band](confidence-band.md) useful for planning how many observations are needed before estimating threshold [probabilities](probability.md) to a chosen simultaneous accuracy.

## ↑ Ancestors (8)

1. [Empirical distribution function](empirical-distribution-function.md)
2. [Cumulative distribution function](cumulative-distribution-function.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Dvoretzky-Kiefer-Wolfowitz inequality](dvoretzky-kiefer-wolfowitz-inequality.md)
