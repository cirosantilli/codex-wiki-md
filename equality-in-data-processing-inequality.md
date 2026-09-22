# Equality in data processing inequality

↑ **Parent:** [Data processing inequality](data-processing-inequality.md)

Under the finite [Markov chain](markov-chain.md) hypothesis $X\to Y\to Z$, the gap identity in the [data processing inequality](data-processing-inequality.md) gives

$$
I(X;Z)=I(X;Y)\quad\Longleftrightarrow\quad I(X;Y\mid Z)=0.
$$

By the zero criterion for [conditional mutual information](conditional-mutual-information.md), equality means that $X$ and $Y$ have [conditional independence](conditional-independence.md) given $Z$. After seeing the processed output, the original observation provides no additional information about $X$. Similarly, equality in the other bound, $I(X;Z)=I(Y;Z)$, holds exactly when $I(Y;Z\mid X)=0$.

Equality does not require retaining every detail of $Y$. Let $X,W$ be [independent](independent-random-variables.md) fair [bits](bit.md), put $Y=(X,W)$, and let the processed output be $Z=X$, the first coordinate of $Y$. This is a [Markov chain](markov-chain.md), and

$$
I(X;Y)=H(X)-H(X\mid X,W)=1-0=1,
\qquad I(X;Z)=I(X;X)=1.
$$

Also $I(X;Y\mid Z)=H(X\mid X)-H(X\mid X,W)=0$. The output discards the entire unrelated [bit](bit.md) $W$, reducing $H(Y)=2$ to $H(Z)=1$, while preserving all [mutual information](mutual-information.md) about $X$. This is what makes equality useful for choosing a compact observation that retains all information about the quantity of interest.

## ↑ Ancestors (7)

1. [Data processing inequality](data-processing-inequality.md)
2. [Mutual information](mutual-information.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Data processing inequality](data-processing-inequality.md)
