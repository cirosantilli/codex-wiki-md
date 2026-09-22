# Entropy rate

↑ **Parent:** [Information theory](information-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entropy_rate)

The [entropy rate](entropy-rate.md) measures average new uncertainty per emitted symbol of a [stochastic process](stochastic-process-split.md). Predictability from earlier symbols can make this much smaller than the [information entropy](information-entropy.md) of one symbol. For example, a [binary Markov source](binary-markov-source.md) can emit a fair [bit](bit.md) at every time while repeating its previous [bit](bit.md) with [probability](probability.md) $7/8$: each individual symbol has one [bit](bit.md) of uncertainty, but the [entropy rate](entropy-rate.md) is only about $0.544$ [bits](bit.md) per symbol.

For a [finite alphabet](finite-alphabet.md) source $X=(X_1,X_2,\ldots)$, define

$$
h(X)=\lim_{n\to\infty}\frac{H(X_1,\ldots,X_n)}n
$$

when the [limit](limit-of-a-function.md) exists. Base-two [logarithms](logarithm.md) give [bits](bit.md) per symbol. Multiplying by a fixed emission frequency $f$ gives $fh(X)$ [bits](bit.md) per unit time; the symbol rate and the uncertainty of the sequence are different inputs. A [strictly stationary process](strictly-stationary-process.md) on a [finite alphabet](finite-alphabet.md) always has an [entropy rate](entropy-rate.md), equal to its [conditional entropy rate](conditional-entropy-rate.md).[§5.5, Definition 5.1 and Theorem 5.5, printed p. 57: block entropy and stationary conditional-entropy limit](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others.md)

For an [independent and identically distributed](independent-and-identically-distributed-random-variables.md) source, the [chain rule for information entropy](chain-rule-for-information-entropy.md) gives $H(X_1,\ldots,X_n)=nH(X_1)$, hence $h(X)=H(X_1)$. With dependence, [conditioning reduces entropy](conditioning-reduces-entropy.md) and makes the past useful. The examples under [Markov information source](markov-information-source.md) show this benefit using exact finite-block calculations.

**Table of contents**

- [Conditional entropy rate](conditional-entropy-rate.md)
- [Entropy rate and coding length](entropy-rate-and-coding-length.md)
- [Shannon's block-entropy approximations](shannon-s-block-entropy-approximations.md)
- [Reliable source encoding at a rate](reliable-source-encoding-at-a-rate.md)
  - [Strong converse for fixed-rate source coding](strong-converse-for-fixed-rate-source-coding.md)
- [Information rate under fixed-length blocking](information-rate-under-fixed-length-blocking.md)

## ↑ Ancestors (5)

1. [Information theory](information-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Binary Markov source](binary-markov-source.md)
- [Conditional entropy rate](conditional-entropy-rate.md)
- [Entropy rate](entropy-rate.md)
- [Entropy rate and coding length](entropy-rate-and-coding-length.md)
- [Entropy rate of a fully observed Markov source](entropy-rate-of-a-fully-observed-markov-source.md)
