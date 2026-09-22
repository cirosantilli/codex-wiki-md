# Probability of a type class

↑ **Parent:** [Method of types](method-of-types.md)

For a string of [empirical distribution](type-information-theory.md) $q$, [independence](independent-random-variables.md) gives

$$
\mathbb P_p(x^n)=\prod_a p(a)^{nq(a)}
=e^{-n[H_e(q)+D_e(q\Vert p)]}.
$$

Multiplying this by the [size of a type class](size-of-a-type-class.md) gives its exact [probability](probability.md). The [entropy bounds for a type class](entropy-bounds-for-a-type-class.md) then imply

$$
(n+1)^{-m}e^{-nD_e(q\Vert p)}\leq
\mathbb P_p(T_n(q))\leq e^{-nD_e(q\Vert p)}.
$$

These bounds apply to one attainable [empirical distribution](type-information-theory.md), not automatically to a tail event containing many classes.[§II, equation (II.1) and Lemma II.2, equation (II.5), printed pp. 2506–2507](the-method-of-types-by-imre-csiszar.md) If $p(a)=0$ but $q(a)>0$, every string in that class is impossible and $D_e(q\Vert p)=+\infty$.

As an exact example, take an [independent and identically distributed](independent-and-identically-distributed-random-variables.md) binary source with $p(1)=1/4$. Each balanced four-symbol string has [probability](probability.md) $(1/4)^2(3/4)^2=9/256$. There are six such strings, so

$$
\boxed{\mathbb P_p(T_4(1/2,1/2))=\frac{54}{256}=0.2109375.}
$$

The [relative entropy](kullback-leibler-divergence.md) is $D_e((1/2,1/2)\Vert(3/4,1/4))=\tfrac12\ln(4/3)$. The exponential upper bound is $e^{-4D_e}=9/16=0.5625$, visibly larger than the exact [probability](probability.md). It captures the cost of an atypical frequency without supplying the exact finite-length prefactor.

For $n=40$, the exact [probability](probability.md) of twenty ones is

$$
\binom{40}{20}(1/4)^{20}(3/4)^{20}\approx0.000397577,
$$

while the exponential upper bound is approximately $0.00317121$. At the source frequency $q(1)=1/4$, [relative entropy](kullback-leibler-divergence.md) is zero and the upper bound is one; the exact [probability](probability.md) of ten ones is only about $0.144364$. A likely neighborhood of frequencies need not give a large [probability](probability.md) to a single exact profile.

<a id="image-relative-entropy-controls-the-rarity-of-an-empirical-frequency"></a>
![](type-class-probability-and-divergence.png)

**[Figure 14](#image-relative-entropy-controls-the-rarity-of-an-empirical-frequency). Relative entropy controls the rarity of an empirical frequency**. Exact [probabilities](probability.md) from the [binomial distribution](binomial-distribution.md) for each possible number of ones in forty [independent and identically distributed](independent-and-identically-distributed-random-variables.md) trials with $p(1)=1/4$, compared with the exponential [relative entropy](kullback-leibler-divergence.md) upper bound. The curves are calculated from a stipulated model, not observed data; the vertical scale is logarithmic.

The striking cancellation is that there are about $e^{nH_e(q)}$ strings in a class, but each costs about $e^{-n[H_e(q)+D_e(q\Vert p)]}$. The [information entropy](information-entropy-split.md) terms cancel, leaving [relative entropy](kullback-leibler-divergence.md) as the rarity exponent. Summing over polynomially many classes preserves that leading exponential scale. This is the elementary counting mechanism behind finite-alphabet versions of [Sanov theorem](sanov-theorem.md) and many [error exponents in hypothesis testing](error-exponents-in-hypothesis-testing.md).

## ↑ Ancestors (7)

1. [Method of types](method-of-types.md)
2. [Type (information theory)](type-information-theory.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
