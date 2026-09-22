# Chain rule for information entropy

↑ **Parent:** [Information entropy](information-entropy-split.md)

For finite [discrete random variables](discrete-random-variable.md), the chain rule counts uncertainty in two stages:

$$
H(X,Y)=H(X)+H(Y\mid X).
$$

The [joint entropy](joint-entropy.md) equals the first variable's [information entropy](information-entropy-split.md) plus the average [conditional entropy](conditional-entropy.md) left in the second. All [logarithms](logarithm.md) here have base two, so the unit is the [bit](bit.md); zero-probability terms contribute zero. The identity holds without assuming [independence](independent-random-variables.md).[section 6, property 5, reprint p. 12: joint entropy as first entropy plus average conditional entropy](a-mathematical-theory-of-communication-by-claude-shannon.md)

Iterating gives $H(X_1,\ldots,X_n)=\sum_iH(X_i\mid X_1,\ldots,X_{i-1})$. The first summand means $H(X_1)$, with no earlier observations. Each later summand counts only the new uncertainty after the preceding [random variables](random-variable-split.md) are known. For [independent random variables](independent-random-variables.md), every term is its ordinary [information entropy](information-entropy-split.md); for dependent ones, adding those ordinary [information entropies](information-entropy-split.md) can count shared uncertainty repeatedly. This is the reason the [chain rule for information entropy](chain-rule-for-information-entropy.md) is useful in [lossless source coding](lossless-source-coding.md) and in calculating an [entropy rate](entropy-rate.md).

A short proof starts from the factorization of the [joint probability mass function](joint-probability-mass-function.md) into a [marginal distribution](marginal-distribution.md) and a [conditional probability](conditional-probability.md):

$$
p_{X,Y}(x,y)=p_X(x)p_{Y\mid X}(y\mid x),\qquad
-\log_2 p_{X,Y}(x,y)=-\log_2 p_X(x)-\log_2p_{Y\mid X}(y\mid x).
$$

Use this only where $p_{X,Y}(x,y)>0$, then average with those joint [probabilities](probability.md). Summing over $y$ in the first term gives $H(X)$; the second is precisely $H(Y\mid X)$. Repeating the same step with a longer [random vector](random-vector.md) proves the iterated identity. Reversing the order also gives $H(X,Y)=H(Y)+H(X\mid Y)$: the two contributions can change with the order, but their total cannot.

**Table of contents**

- [Correlated binary variables](correlated-binary-variables.md)

## ↑ Ancestors (6)

1. [Information entropy](information-entropy-split.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (35)

- [Chain decomposition of total correlation](chain-decomposition-of-total-correlation.md)
- [Chain rule for information entropy](chain-rule-for-information-entropy.md)
- [Conditional entropy](conditional-entropy.md)
- [Conditional entropy rate](conditional-entropy-rate.md)
- [Correlated binary variables](correlated-binary-variables.md)
- [Entropy rate](entropy-rate.md)
- [Entropy rate of a fully observed Markov source](entropy-rate-of-a-fully-observed-markov-source.md)
- [Independent revelation of a binary variable](independent-revelation-of-a-binary-variable.md)
- [Information entropy](information-entropy-split.md)
- [Joint entropy](joint-entropy.md)
- [Madiman–Tetali entropy inequality](madiman-tetali-entropy-inequality.md)
- [Monotonicity of normalized subset entropies](monotonicity-of-normalized-subset-entropies.md)
- [Noisy parity total correlation](noisy-parity-total-correlation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-13/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-15/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-108/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-108/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-161/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-161/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-224/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/4/d/solution.md)
- [Shearer's inequality](shearer-s-inequality.md)
- [Subadditivity of information entropy](subadditivity-of-information-entropy.md)
