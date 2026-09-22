# Haldane mapping function

↑ **Parent:** [Genetic map](genetic-map.md)

The Haldane mapping function connects additive [genetic map](genetic-map.md) distance to endpoint [recombination fraction](recombination-fraction.md) in a toy model with no [crossover interference](crossover-interference.md). Specify the model directly along a transmitted [chromatid](chromatid.md): the exchange count $N$ in the interval has a [Poisson distribution](poisson-distribution.md) with [expected value](expected-value.md) $d$, where $d$ is the distance in [morgans](morgan-unit.md). Counts in disjoint intervals are [independent random variables](independent-random-variables.md). This is the transmitted-[chromatid](chromatid.md) convention; $d$ is not the mean number of exchanges across all four [chromatids](chromatid.md) in [meiosis](meiosis.md).

An odd exchange count changes parental phase. Summing the odd terms of the [Poisson distribution](poisson-distribution.md) gives

$$
r=P(N\text{ is odd})=e^{-d}\sum_{k=0}^{\infty}\frac{d^{2k+1}}{(2k+1)!}=\frac{1-e^{-2d}}{2}.
$$

For $0\le r<1/2$, the inverse and short-interval approximation are

$$
d=-\frac12\log(1-2r),\qquad r=d-d^2+O(d^3).
$$

Here $\log$ is the [natural logarithm](natural-logarithm.md). At $d=0.2$, the [recombination fraction](recombination-fraction.md) is $0.16483997698$; at $r=0.2$, the distance is $0.2554128119$ [morgans](morgan-unit.md), or about $25.5413$ [centimorgans](centimorgan.md). The linear approximation $r\approx d$ is useful only near zero. The [recombination fraction](recombination-fraction.md) approaches $1/2$ as $d$ grows; $r=1/2$ has no finite inverse in this model.

<a id="image-haldane-mapping-function-versus-the-short-interval-approximation-genetic-map-distance-keeps-growing-while-the-recombination-fraction-approaches-one-half"></a>
![](recombination-fraction-map-distance.png)

**[Figure 85](#image-haldane-mapping-function-versus-the-short-interval-approximation-genetic-map-distance-keeps-growing-while-the-recombination-fraction-approaches-one-half). Haldane mapping function versus the short-interval approximation: genetic map distance keeps growing while the recombination fraction approaches one half**.

The model is a useful baseline, not a universal rule for every interval during [meiosis](meiosis.md). [Crossover interference](crossover-interference.md) can change the relationship between distance and [recombination fraction](recombination-fraction.md). For the count convention and assumptions, see [Weeks, Tang and Kwon (2009): genetic map functions and exchange-count conventions](https://pmc.ncbi.nlm.nih.gov/articles/PMC2704907/). Haldane's original paper is bibliographically recorded as _The combination of linkage values, and the calculation of distances between the loci of linked factors_, _Journal of Genetics_ 8 (1919), 299–309, in [Selected Genetics Papers of J. B. S. Haldane, edited by K. Dronamraju (1990), contents](https://jbshaldane.org/books/1990-Selected-Genetics-Papers/index.html).

## ↑ Ancestors (5)

1. [Genetic map](genetic-map.md)
2. [Genetic linkage](genetic-linkage.md)
3. [Genetics](genetics.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Crossover interference](crossover-interference.md)
- [Genetic map](genetic-map.md)
- [Genetic recombination](genetic-recombination.md)
- [Haldane mapping function](haldane-mapping-function.md)
- [Recombination fraction](recombination-fraction.md)
