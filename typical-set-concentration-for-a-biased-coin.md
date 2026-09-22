# Typical-set concentration for a biased coin

↑ **Parent:** [Bernoulli typical-set example](bernoulli-typical-set-example.md)

The count $K_n$ has [binomial distribution](binomial-distribution.md) with [mean](expected-value-split.md) $n/4$ and [variance](variance-split.md) $3n/16$. The [information content](information-content.md) per symbol is an affine function of $K_n/n$, so its [variance](variance-split.md) is

$$
\operatorname{Var}\left(\frac{\imath(K_n)}n\right)
=\frac{3(\log_2 3)^2}{16n}.
$$

[Chebyshev's inequality](chebyshev-s-inequality.md) therefore gives the finite-sample lower bound

$$
P(T_\varepsilon^{(n)})\geq
\max\left(0,1-\frac{3(\log_2 3)^2}{16n\varepsilon^2}\right).
$$

The bound is often loose, but it proves that every fixed positive tolerance eventually captures nearly all the [probability](probability.md). Direct summation of the [binomial distribution](binomial-distribution.md)'s [probability masses](probability-mass.md) gives $P(T_{0.1}^{(640)})\approx0.999779$. A finite sample does not need to have a nearly full [typical set](typical-set.md): the 40-symbol example above captures only about $0.639$.

<a id="image-longer-biased-coin-messages-concentrate-in-typical-sets-with-controlled-size"></a>
![](typical-set-concentration-and-size-bounds.png)

**[Figure 28](#image-longer-biased-coin-messages-concentrate-in-typical-sets-with-controlled-size). Longer biased-coin messages concentrate in typical sets with controlled size**. The left plot compares exact [typical set](typical-set.md) probabilities with the lower bound from [Chebyshev's inequality](chebyshev-s-inequality.md). The right shows $n^{-1}\log_2|T_{0.1}^{(n)}|$ and its finite-sample bounds. The tolerance stays fixed; the curve is not asserted to converge to exactly $H$. All points are exact finite-model calculations.

## ↑ Ancestors (7)

1. [Bernoulli typical-set example](bernoulli-typical-set-example.md)
2. [Asymptotic equipartition property](asymptotic-equipartition-property.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
