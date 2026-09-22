# Cross-entropy

↑ **Parent:** [Information entropy](information-entropy-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cross-entropy)

[Cross-entropy](cross-entropy.md) measures the average [logarithmic loss](logarithmic-loss.md) incurred when outcomes follow one [probability distribution](probability-distribution-split.md) $P$, but a model assigns [probabilities](probability.md) using another [probability distribution](probability-distribution-split.md) $Q$. For a finite [alphabet](alphabet.md), write their [probability mass functions](probability-mass-function.md) as $p_i$ and $q_i$. With base-two [logarithms](logarithm.md),

$$
H(P,Q)=-\sum_{i:p_i>0}p_i\log_2 q_i=\mathbb E_P[-\log_2 q(X)].
$$

The expectation is under the true or stipulated source law $P$, rather than the model $Q$. Terms with $p_i=0$ contribute nothing. If $p_i>0$ but $q_i=0$ for any outcome, the [cross-entropy](cross-entropy.md) is $+\infty$: the model rules out an event that can occur. The result is measured in [bits](bit.md); [natural logarithms](natural-logarithm.md) give [nats](nat-unit.md).

The useful identity is [cross-entropy equals entropy plus relative entropy](cross-entropy-equals-entropy-plus-relative-entropy.md):

$$
\boxed{H(P,Q)=H(P)+D_{\mathrm{KL}}(P\Vert Q).}
$$

The source's [information entropy](information-entropy-split.md) $H(P)$ is the baseline uncertainty. The [Kullback-Leibler divergence](kullback-leibler-divergence.md) is the extra average cost of a mismatched model, with the true law first and model second. Thus optimizing $Q$ for a fixed $P$ reduces the mismatch, rather than changing the source's own uncertainty. For finite [alphabets](alphabet.md), the minimum is $H(P)$, attained exactly at $Q=P$.

Take a three-symbol source with $P=(1/2,1/4,1/4)$. A matched binary [prefix code](prefix-code.md) assigns $A\mapsto0$, $B\mapsto10$, $C\mapsto11$, with lengths $(1,2,2)$. A mismatched [prefix code](prefix-code.md) instead assigns $A\mapsto10$, $B\mapsto11$, $C\mapsto0$, with lengths $(2,2,1)$, corresponding to $Q=(1/4,1/4,1/2)$. Both [prefix codes](prefix-code.md) decode exactly, but the most common symbol is shorter in the matched code. Under the same source $P$,

$$
\begin{aligned}
H(P)&=\tfrac12\cdot1+\tfrac14\cdot2+\tfrac14\cdot2=\tfrac32,\\
H(P,Q)&=\tfrac12\cdot2+\tfrac14\cdot2+\tfrac14\cdot1=\tfrac74,\\
D_{\mathrm{KL}}(P\Vert Q)&=\tfrac12\log_2 2+\tfrac14\log_2 1+\tfrac14\log_2(1/2)=\tfrac14.
\end{aligned}
$$

**The mismatched code costs an extra (1/4) bit per source symbol on average.** No information is lost; the penalty is inefficient representation of this source. The [mismatch penalty in lossless coding](mismatch-penalty-in-lossless-coding.md) explains when this coding interpretation is exact.

<a id="image-two-lossless-prefix-codes-have-different-average-lengths-for-the-same-source"></a>
![](cross-entropy-mismatched-prefix-codes.png)

**[Figure 1](#image-two-lossless-prefix-codes-have-different-average-lengths-for-the-same-source). Two lossless prefix codes have different average lengths for the same source**. Both sets of [codewords](codeword.md) are [prefix codes](prefix-code.md). The source [probabilities](probability.md) are fixed at $(1/2,1/4,1/4)$. Each colored contribution is source [probability](probability.md) times [codeword length](codeword-length.md); changing which symbol receives the shortest word increases the total from $3/2$ to $7/4$ [bits](bit.md) per source symbol.

[Cross-entropy](cross-entropy.md) is also useful when evaluating a [predictive distribution](predictive-distribution.md). A report that places tiny [probability](probability.md) on the realized outcome receives a large [logarithmic loss](logarithmic-loss.md), even when it usually predicts the most common outcome correctly. The loss convention is the negative of the reward convention in the [logarithmic scoring rule](logarithmic-scoring-rule.md). Its expected loss is uniquely minimized by the correct [probability distribution](probability-distribution-split.md), making it a [strictly proper scoring rule](strictly-proper-scoring-rule.md). [Strictly Proper Scoring Rules, Prediction, and Estimation by Tilmann Gneiting and others](strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others.md) treats this connection in §3.1, Example 3; its discussion uses rewards, so the signs are reversed for the losses here.[Strictly Proper Scoring Rules, Prediction, and Estimation by Tilmann Gneiting and others](strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others.md)

[I. J. Good](i-j-good.md)'s [Rational Decisions by I. J. Good](rational-decisions-by-i-j-good.md) appeared in 1952. Its published summary describes a method for encouraging accurate [probability](probability.md) estimates and a connection with [information theory](information-theory-split.md). [Strictly Proper Scoring Rules, Prediction, and Estimation by Tilmann Gneiting and others](strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others.md) traces the [logarithmic scoring rule](logarithmic-scoring-rule.md) at least as far back as this 1952 paper.[Rational Decisions by I. J. Good](rational-decisions-by-i-j-good.md)

**Table of contents**

- [Cross-entropy equals entropy plus relative entropy](cross-entropy-equals-entropy-plus-relative-entropy.md)
- [Mismatch penalty in lossless coding](mismatch-penalty-in-lossless-coding.md)
- [Binary cross-entropy](binary-cross-entropy.md)
- [Empirical cross-entropy](empirical-cross-entropy.md)
  - [Cross-entropy and maximum likelihood](cross-entropy-and-maximum-likelihood.md)

## ↑ Ancestors (6)

1. [Information entropy](information-entropy-split.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Binary cross-entropy](binary-cross-entropy.md)
- [Cross-entropy](cross-entropy.md)
- [Cross-entropy equals entropy plus relative entropy](cross-entropy-equals-entropy-plus-relative-entropy.md)
- [Kullback-Leibler divergence](kullback-leibler-divergence.md)
- [Logarithmic loss](logarithmic-loss.md)
- [Mismatch penalty in lossless coding](mismatch-penalty-in-lossless-coding.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-3/section-f/47/c/solution.md)
