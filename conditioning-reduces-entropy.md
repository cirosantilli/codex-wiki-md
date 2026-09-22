# Conditioning reduces entropy

↑ **Parent:** [Conditional entropy](conditional-entropy.md)

For finite [discrete random variables](discrete-random-variable.md) $X,Y$, knowing $Y$ reduces the [information entropy](information-entropy-split.md) of $X$ on average:

$$
H(X\mid Y)=\sum_{y:p_Y(y)>0}p_Y(y)H(X\mid Y=y)\leq H(X).
$$

Equality holds exactly when $X$ and $Y$ are [independent random variables](independent-random-variables.md). The average over observations is essential: $H(X\mid Y=y)$ can exceed $H(X)$ for a particular $y$. All [logarithms](logarithm.md) here have base two, giving [bits](bit.md), and zero-probability terms contribute zero.[Definition 1.3, printed p. 8; Theorem 1.1(4), printed p. 10](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-1-information-measures-entropy-and-divergence.md)

For [Bayesian inference](bayesian-statistics-split.md), this compares a [prior distribution](prior-probability.md) with the [posterior distributions](bayesian-posterior.md) produced by possible observations. An unexpected report can make previously unlikely alternatives plausible, while useful reports reduce uncertainty overall. For [lossless source coding](lossless-source-coding.md), an observation shared by [encoder](channel-encoder.md) and [decoder](channel-decoder.md) lets them choose descriptions for the appropriate [conditional distribution](conditional-distribution.md); sending that observation also has a cost. The example below makes both the saving and that cost explicit.

In [A Mathematical Theory of Communication by Claude Shannon](a-mathematical-theory-of-communication-by-claude-shannon.md) (1948), the definition of [conditional entropy](conditional-entropy.md) is already an average over observations, followed by the inequality and its [independence](independent-random-variables.md) condition in section 6, property 6. The phrase “knowledge reduces uncertainty” must be read with that averaging convention.[p. 12; title page identifies C. E. Shannon and the 1948 journal publication](a-mathematical-theory-of-communication-by-claude-shannon.md)

**Table of contents**

- [An observation can increase entropy](an-observation-can-increase-entropy.md)
- [Independent revelation of a binary variable](independent-revelation-of-a-binary-variable.md)
- [Additional conditioning reduces entropy](additional-conditioning-reduces-entropy.md)
- [Conditioning and differential entropy](conditioning-and-differential-entropy.md)

## ↑ Ancestors (6)

1. [Conditional entropy](conditional-entropy.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (33)

- [Conditional entropy](conditional-entropy.md)
- [Conditional entropy of a countable measurable partition](conditional-entropy-of-a-countable-measurable-partition.md)
- [Conditional entropy of finite measurable partitions](conditional-entropy-of-finite-measurable-partitions.md)
- [Conditional entropy rate](conditional-entropy-rate.md)
- [Conditional mutual information](conditional-mutual-information.md)
- [Conditioned entropic Ruzsa distance of a summand](conditioned-entropic-ruzsa-distance-of-a-summand.md)
- [Entropy rate](entropy-rate.md)
- [Fano's inequality via an error indicator](fano-s-inequality-via-an-error-indicator.md)
- [Joint entropy](joint-entropy.md)
- [Madiman–Tetali entropy inequality](madiman-tetali-entropy-inequality.md)
- [Monotonicity of normalized block entropy](monotonicity-of-normalized-block-entropy.md)
- [Monotonicity of normalized subset entropies](monotonicity-of-normalized-subset-entropies.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-13/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-15/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-12/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-108/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-108/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-108/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/3g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-108/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-161/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-224/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/12i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/4/i/solution.md)
- [Shearer's inequality](shearer-s-inequality.md)
- [Subadditivity of information entropy](subadditivity-of-information-entropy.md)
