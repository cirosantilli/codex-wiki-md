# Bernoulli typical-set example

↑ **Parent:** [Asymptotic equipartition property](asymptotic-equipartition-property.md)

Take an [IID random variable](independent-and-identically-distributed-random-variables.md) source of [bits](bit.md) with $P(X_j=1)=1/4$. Its [binary entropy](binary-entropy.md) is

$$
H=h_2(1/4)=-\frac14\log_2\frac14-\frac34\log_2\frac34
\approx0.811278\text{ bits per symbol}.
$$

A word of length $n$ containing $k$ ones has [probability](probability.md) $(1/4)^k(3/4)^{n-k}$. Its [information content](information-content.md) per symbol is

$$
\frac{\imath(k)}n=\log_2\frac43+\frac kn\log_2 3.
$$

Thus [weakly typical sequences](weakly-typical-sequence.md) for this biased source have $k/n$ near $1/4$. With tolerance $\varepsilon=0.1$ [bits](bit.md) per symbol, the exact condition is

$$
\left|\frac kn-\frac14\right|\leq\frac{0.1}{\log_2 3}.
$$

For $n=40$, this includes exactly $k=8,9,10,11,12$. There are $\binom{40}{k}$ words with each count: a [type class](type-class.md) with that many possible orderings. Summing the counts and their [probability masses](probability-mass.md) gives

$$
\boxed{|T_{0.1}^{(40)}|=9\,096\,659\,013,\qquad
P(T_{0.1}^{(40)})\approx0.638912.}
$$

These are fewer than one percent of the $2^{40}$ possible words, yet they carry nearly 64 percent of the [probability](probability.md). The most likely individual word is all zeros, with [probability](probability.md) $(3/4)^{40}\approx1.006\times10^{-5}$; it is outside this [typical set](typical-set.md). No contradiction is involved: the [type classes](type-class.md) near ten ones each contain many more individual words.

<a id="image-the-most-likely-individual-word-differs-from-the-counts-carrying-most-probability"></a>
![](typical-set-individual-words-and-count-mass.png)

**[Figure 27](#image-the-most-likely-individual-word-differs-from-the-counts-carrying-most-probability). The most likely individual word differs from the counts carrying most probability**. The left plot gives the [information content](information-content.md) of one word with each number of ones. The right includes the [binomial coefficient](binomial-coefficient-split.md) counting every such word, giving the exact [binomial distribution](binomial-distribution.md) of the count. Both use $n=40$, $p=1/4$; the green band marks the [typical set](typical-set.md) with tolerance $0.1$ [bits](bit.md) per symbol.

**Table of contents**

- [Typical-set concentration for a biased coin](typical-set-concentration-for-a-biased-coin.md)
- [Typical-set indexing example](typical-set-indexing-example.md)

## ↑ Ancestors (6)

1. [Asymptotic equipartition property](asymptotic-equipartition-property.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Asymptotic equipartition property](asymptotic-equipartition-property.md)
