# Bit-position information in a binary channel

↑ **Parent:** [Conditional mutual information](conditional-mutual-information.md)

Suppose a fair input bit $X$ is independent of a publicly known channel-position label $J$. At position $j$, let the channel be a [binary symmetric channel](binary-symmetric-channel.md) with error probability $p_j$. Forgetting $J$ gives a binary symmetric channel with error $\overline p=\mathbb E p_J$. Therefore

$$
I(X;Y\mid J)=1-\mathbb E h_2(p_J),\qquad
I(X;Y)=1-h_2(\mathbb E p_J).
$$

The [chain rule for mutual information](chain-rule-for-mutual-information.md) and $I(X;J)=0$ show that their difference is the nonnegative [conditional mutual information](conditional-mutual-information.md) $I(X;J\mid Y)$. Equivalently, the inequality follows from concavity of [binary entropy](binary-entropy.md). For $p_0=1/5,p_1=0$ with equal position weights, the known-position value is $0.639036$ bits and the pooled value is $0.531004$ bits. These quantities answer different statistical questions.

## ↑ Ancestors (7)

1. [Conditional mutual information](conditional-mutual-information.md)
2. [Mutual information](mutual-information.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2006/7/3/solution.md)
