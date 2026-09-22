# Innovations in a binary Markov source

↑ **Parent:** [Binary Markov source](binary-markov-source.md)

Generate the [binary Markov source](binary-markov-source.md) by taking [independent and identically distributed](independent-and-identically-distributed-random-variables.md) [Bernoulli random variables](bernoulli-distribution.md) $Z_2,Z_3,\ldots$ of parameter $q$, independent of a fair initial [bit](bit.md), and setting $X_n=X_{n-1}\oplus Z_n$. Here $\oplus$ is [exclusive or](exclusive-or.md). Each $Z_n$ is the unpredictable flip decision.

The transformation between $(X_1,\ldots,X_n)$ and $(X_1,Z_2,\ldots,Z_n)$ is a [bijection](bijection.md). It preserves [information entropy](information-entropy.md), so

$$
H(X_1,\ldots,X_n)=H(X_1,Z_2,\ldots,Z_n)=1+(n-1)h_2(q).
$$

Sending the initial [bit](bit.md) and encoding the innovation sequence describes every source word exactly. This does not by itself specify a practical compressor, but it identifies the uncertainty which a [prefix code](prefix-code.md) or other [lossless source coding](lossless-source-coding.md) method must handle.

For a word with $k$ flips among its $n-1$ transitions,

$$
\mathbb P(X_1=x_1,\ldots,X_n=x_n)=\frac12q^k(1-q)^{n-1-k}.
$$

There are $2\binom{n-1}{k}$ such words: choose the initial [bit](bit.md) and the flip positions. At $q=1/8$ and $n=16$, each constant word has [probability](probability.md) $(1/2)(7/8)^{15}\simeq0.06746691$, whereas an independent fair source gives each word [probability](probability.md) $2^{-16}$. Equal marginal [probabilities](probability.md) plainly do not imply equal word [probabilities](probability.md).

## ↑ Ancestors (8)

1. [Binary Markov source](binary-markov-source.md)
2. [Fully observed Markov source](fully-observed-markov-source.md)
3. [Markov information source](markov-information-source.md)
4. [Information theory](information-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Binary Markov source](binary-markov-source.md)
