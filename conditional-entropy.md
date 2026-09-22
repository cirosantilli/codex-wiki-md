# Conditional entropy

↑ **Parent:** [Information theory](information-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conditional_entropy)

For finite [discrete random variables](discrete-random-variable.md), conditional entropy is the average remaining [information entropy](information-entropy-split.md) of $Y$ after the value of $X$ is known:

$$
H(Y\mid X)=\sum_{x:p_X(x)>0}p_X(x)H(Y\mid X=x).
$$

Each observation $X=x$ changes the [probability distribution](probability-distribution-split.md) used to describe $Y$; the average weights that uncertainty by how often the observation occurs. An observation can increase uncertainty for one particular outcome, even though [conditioning reduces entropy](conditioning-reduces-entropy.md) on average for finite variables.

For example, let $Y$ choose $A,B,C,D$ with [probabilities](probability.md) $1/2,1/4,1/8,1/8$, and let $X$ report whether $Y=A$. If it reports yes, there is no remaining uncertainty. Otherwise the conditional [probabilities](probability.md) are $1/2,1/4,1/4$, whose [information entropy](information-entropy-split.md) is $3/2$ [bits](bit.md). The two reports each occur with [probability](probability.md) $1/2$, so $H(Y\mid X)=3/4$ of a [bit](bit.md). The original uncertainty was $7/4$ [bits](bit.md): this observation removes exactly one [bit](bit.md) on average.

If $Y$ is a [function](function-split.md) of $X$, then $H(Y\mid X)=0$: the observation determines the answer. If $X$ and $Y$ are [independent random variables](independent-random-variables.md), then $H(Y\mid X)=H(Y)$: the observation gives no improvement. These endpoints make [conditional entropy](conditional-entropy.md) useful for separating relevant observations from irrelevant ones. They also lead to the [chain rule for information entropy](chain-rule-for-information-entropy.md), $H(X,Y)=H(X)+H(Y\mid X)$, which counts the first uncertainty and the remaining uncertainty without double counting.

**Table of contents**

- [Equality in the entropy conditioning inequality](equality-in-the-entropy-conditioning-inequality.md)
- [Chain rule for conditional entropy](chain-rule-for-conditional-entropy.md)
- [Conditional entropy under a deterministic change of variables](conditional-entropy-under-a-deterministic-change-of-variables.md)
- [Conditioning reduces entropy](conditioning-reduces-entropy.md)
  - [An observation can increase entropy](an-observation-can-increase-entropy.md)
  - [Independent revelation of a binary variable](independent-revelation-of-a-binary-variable.md)
  - [Additional conditioning reduces entropy](additional-conditioning-reduces-entropy.md)
  - [Conditioning and differential entropy](conditioning-and-differential-entropy.md)
- [Fano's inequality](fano-s-inequality.md)
  - [Fano's inequality via an error indicator](fano-s-inequality-via-an-error-indicator.md)
  - [List-decoding Fano inequality](list-decoding-fano-inequality.md)
- [Entropy of a sum of independent finite-group variables](entropy-of-a-sum-of-independent-finite-group-variables.md)

## ↑ Ancestors (5)

1. [Information theory](information-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (39)

- [An observation can increase entropy](an-observation-can-increase-entropy.md)
- [Binary rate-distortion function](binary-rate-distortion-function.md)
- [Chain rule for information entropy](chain-rule-for-information-entropy.md)
- [Chain rule for mutual information](chain-rule-for-mutual-information.md)
- [Conditional entropy](conditional-entropy.md)
- [Conditional mutual information](conditional-mutual-information.md)
- [Conditioning reduces entropy](conditioning-reduces-entropy.md)
- [Correlated binary variables](correlated-binary-variables.md)
- [Cyclic ternary channel capacity](cyclic-ternary-channel-capacity.md)
- [Entropy monotonicity under independent addition](entropy-monotonicity-under-independent-addition.md)
- [Entropy rate of a fully observed Markov source](entropy-rate-of-a-fully-observed-markov-source.md)
- [Fano's inequality](fano-s-inequality.md)
- [Flips versus erasures in a binary channel](flips-versus-erasures-in-a-binary-channel.md)
- [Independent revelation of a binary variable](independent-revelation-of-a-binary-variable.md)
- [Information entropy](information-entropy-split.md)
- [Information theory](information-theory-split.md)
- [Joint entropy](joint-entropy.md)
- [List-decoding Fano inequality](list-decoding-fano-inequality.md)
- [Min-entropy](min-entropy.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/4j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/2/ii/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/2/ii/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/5/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-108/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/4/c/solution.md)
