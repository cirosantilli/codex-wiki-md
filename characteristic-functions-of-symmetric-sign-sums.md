# Characteristic functions of symmetric sign sums

↑ **Parent:** [Characteristic function of a sum of independent variables](characteristic-function-of-a-sum-of-independent-variables.md)

Let $X_1,X_2,\ldots$ be [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) taking $-1$ and $1$ with equal [probabilities](probability.md), the [Rademacher distribution](rademacher-distribution.md). The two opposite [complex exponentials](complex-exponential-function.md) give $\varphi_X(t)=(e^{it}+e^{-it})/2=\cos t$. Their [expected value](expected-value-split.md) is zero and their [variance](variance-split.md) is one. For $S_n=\sum_{j=1}^nX_j$, the [characteristic functions](characteristic-function-split.md) of its [sample mean](sample-mean.md) and its [variance normalization](variance-normalization.md) are respectively

$$
\varphi_{S_n/n}(t)=\cos(t/n)^n,\qquad
\varphi_{S_n/\sqrt n}(t)=\cos(t/\sqrt n)^n.
$$

For each fixed $t$, the bases are positive for all sufficiently large $n$. The [Taylor expansion](taylor-expansion.md) $\log\cos u=-u^2/2+O(u^4)$ at zero then gives

$$
n\log\cos(t/n)=-\frac{t^2}{2n}+O(n^{-3})\longrightarrow0,
\qquad
n\log\cos(t/\sqrt n)=-\frac{t^2}{2}+O(n^{-1})\longrightarrow-\frac{t^2}{2}.
$$

Exponentiating proves the two displayed pointwise limits. The first limit is the [characteristic function](characteristic-function-split.md) of the constant zero; the second is that of the [standard normal distribution](standard-normal-distribution.md). The [Lévy continuity theorem](levy-continuity-theorem.md) gives the corresponding [convergence in distribution](convergence-in-distribution.md) statements. Averaging has [variance](variance-split.md) $1/n$, whereas dividing the sum by $\sqrt n$ preserves [variance](variance-split.md) one. This sign calculation illustrates why the [law of large numbers](law-of-large-numbers.md) and the [central limit theorem](central-limit-theorem.md) use different scales; it is not a proof for arbitrary [probability distributions](probability-distribution-split.md).

## ↑ Ancestors (7)

1. [Characteristic function of a sum of independent variables](characteristic-function-of-a-sum-of-independent-variables.md)
2. [Characteristic function](characteristic-function-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
