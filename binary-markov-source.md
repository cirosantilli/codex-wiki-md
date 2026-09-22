# Binary Markov source

↑ **Parent:** [Fully observed Markov source](fully-observed-markov-source.md)

Take the [alphabet](alphabet.md) $\{0,1\}$, fair initial [bit](bit.md) $X_1$, and [transition matrix](stochastic-matrix.md)

$$
P=\begin{pmatrix}1-q&q\\q&1-q\end{pmatrix},\qquad 0\leq q\leq1.
$$

The [stationary distribution](stationary-distribution.md) is $(1/2,1/2)$. Every emitted symbol is a fair [bit](bit.md), while the next symbol flips the previous one with [probability](probability.md) $q$. For $q<1/2$, repeating the previous symbol is the better one-step prediction; for $q>1/2$, predicting its opposite is better. The resulting minimum next-symbol error [probability](probability.md) is $\min(q,1-q)$, compared with $1/2$ when no history is used.

Given either state, the next-symbol [information entropy](information-entropy.md) is $h_2(q)$. Thus

$$
H(X_n)=1,\qquad H(X_n\mid X_1,\ldots,X_{n-1})=h_2(q)\quad(n\geq2),\qquad
\boxed{h(X)=h_2(q).}
$$

At $q=1/8$, the best next-symbol prediction succeeds with [probability](probability.md) $7/8$, and the [entropy rate](entropy-rate.md) is about $0.54356444$ [bits](bit.md) per symbol. The adjacent symbols share [mutual information](mutual-information.md) $I(X_1;X_2)=1-h_2(q)\simeq0.45643556$ [bits](bit.md). This is useful structure even though the single-symbol counts reveal no bias.

<a id="image-a-persistent-fair-bit-source-reveals-its-new-randomness-through-the-flip-sequence"></a>
![](entropy-rate-binary-source-and-innovations.png)

**[Figure 32](#image-a-persistent-fair-bit-source-reveals-its-new-randomness-through-the-flip-sequence). A persistent fair-bit source reveals its new randomness through the flip sequence**. Original simulated [sample paths](sample-path.md) with a fixed random seed. The top row is a stationary [binary Markov source](binary-markov-source.md) with $q=1/8$; the middle row records [innovations in a binary Markov source](innovations-in-a-binary-markov-source.md), marking whether each symbol differs from its predecessor. The bottom row is an independent fair-bit comparison. The marginal theoretical [probabilities](probability.md) are $1/2$ for both displayed source processes; finite empirical counts need not be exactly equal. These traces illustrate the stipulated models and are not measured data or a proof of the [entropy rate](entropy-rate.md).

At $q=0$, the random initial [bit](bit.md) is repeated forever; at $q=1$, it alternates forever. Both have $H(X_1,\ldots,X_n)=1$ and zero [entropy rate](entropy-rate.md). At $q=1/2$, the symbols are [independent and identically distributed](independent-and-identically-distributed-random-variables.md) fair [bits](bit.md), giving [entropy rate](entropy-rate.md) one. Zero rate therefore need not mean that the initial choice was deterministic.

**Table of contents**

- [Innovations in a binary Markov source](innovations-in-a-binary-markov-source.md)

## ↑ Ancestors (7)

1. [Fully observed Markov source](fully-observed-markov-source.md)
2. [Markov information source](markov-information-source.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Binary Markov source](binary-markov-source.md)
- [Entropy rate](entropy-rate.md)
- [Entropy rate and coding length](entropy-rate-and-coding-length.md)
- [Innovations in a binary Markov source](innovations-in-a-binary-markov-source.md)
- [Shannon's block-entropy approximations](shannon-s-block-entropy-approximations.md)
