# Sampling without replacement

↑ **Parent:** [Probability sampling](probability-sampling.md)

[Sampling without replacement](sampling-without-replacement.md) selects distinct labelled units: after a unit is selected it is unavailable for the remaining draws. Distinct labels can carry equal numerical values, so repeated values do not necessarily imply a repeated unit. The rule alone does not specify selection [probabilities](probability.md); a procedure favoring particular units is still [sampling without replacement](sampling-without-replacement.md) but need not be [simple random sampling](simple-random-sampling.md).

In uniform sequential [sampling without replacement](sampling-without-replacement.md), the next label is chosen uniformly among those remaining. For a population of $N$ labels, any ordered sequence of $n$ distinct labels has [probability](probability.md) $1/[N(N-1)\cdots(N-n+1)]$. Each size-$n$ [subset](subset.md) has $n!$ possible orders, so its [probability](probability.md) is $\binom Nn^{-1}$. This gives the fixed-size [simple random sampling](simple-random-sampling.md) design. Equivalently, take the first $n$ labels of a uniformly random [permutation](permutation.md). Restricting a uniformly random [permutation](permutation.md) to a specified label set preserves uniformity; biased modulo mappings should not replace uniform selection.

The draw positions have identical marginal [probability distributions](probability-distribution-split.md), but exhibit [statistical dependence](statistical-dependence.md). If the first label is $i$, the [conditional probability](conditional-probability.md) that the second label is $i$ is zero, whereas its marginal [probability](probability.md) is $1/N$. Thus these draws are not [independent and identically distributed](independent-and-identically-distributed-random-variables.md) when $N>1$ and $n>1$. For a marked subset of labels, counting size-$n$ [subsets](subset.md) with [binomial coefficients](binomial-coefficient-split.md) gives the [hypergeometric distribution](hypergeometric-distribution.md). The resulting negative [covariance](covariance.md) explains the [finite population correction](finite-population-correction.md) for both counts and [sample means](sample-mean.md).

**Table of contents**

- [Marginal and pair probabilities in sampling without replacement](marginal-and-pair-probabilities-in-sampling-without-replacement.md)
- [First return to equal counts in sampling without replacement](first-return-to-equal-counts-in-sampling-without-replacement.md)
- [First marked item in a random permutation](first-marked-item-in-a-random-permutation.md)

## ↑ Ancestors (6)

1. [Probability sampling](probability-sampling.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (31)

- [Capture-recapture model](capture-recapture-model.md)
- [Complement rule of probability](complement-rule-of-probability.md)
- [Factorial](factorial.md)
- [Finite population correction](finite-population-correction.md)
- [First marked item in a random permutation](first-marked-item-in-a-random-permutation.md)
- [First return to equal counts in sampling without replacement](first-return-to-equal-counts-in-sampling-without-replacement.md)
- [Hypergeometric distribution](hypergeometric-distribution.md)
- [Mark and recapture](mark-and-recapture.md)
- [Memorylessness of the geometric distribution](memorylessness-of-the-geometric-distribution.md)
- [Multivariate hypergeometric distribution](multivariate-hypergeometric-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-2/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/18/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/18/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/18/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-1/18/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/16/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/16/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1/16/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1/16/a/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/16/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/16/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/16/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/16/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/12/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/12/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/12/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/12/e/ii/solution.md)
- [Sample mean under simple random sampling](sample-mean-under-simple-random-sampling.md)
- [Sampling without replacement](sampling-without-replacement.md)
- [Sampling without replacement need not be independent](sampling-without-replacement-need-not-be-independent.md)
- [Simple random sampling](simple-random-sampling.md)
