# Bootstrap sample

↑ **Parent:** [Bootstrapping (statistics)](bootstrapping-statistics.md)

A [bootstrap sample](bootstrap-sample.md) of size $n$ is drawn by [sampling with replacement](sampling-with-replacement.md) from the $n$ observed data slots. Some observations occur repeatedly. For a given slot, every draw misses it with [probability](probability.md) $1-1/n$, so its omission [probability](probability.md) after $n$ [independent](independent-random-variables.md) draws is

$$
\mathbb P_*(N_i=0)=\left(1-\frac1n\right)^n\longrightarrow e^{-1}.
$$

By [linearity of expectation](linearity-of-expectation.md), the expected number of omitted slots is $n(1-1/n)^n$, whether or not their omission events are [independent](independent-random-variables.md). For the three-observation [exact bootstrap distribution for three observations](exact-bootstrap-distribution-for-three-observations.md), an individual slot is omitted with [probability](probability.md) $8/27$ and the expected number of omitted slots is $8/9$. This finite-sample calculation explains both repeated values and incomplete coverage; $e^{-1}$ is a limiting expected proportion, not an exact fraction in every resample.

**Table of contents**

- [Wild bootstrap](wild-bootstrap.md)
- [Paired bootstrap](paired-bootstrap.md)
- [Conditional bootstrap variance of a sample mean](conditional-bootstrap-variance-of-a-sample-mean.md)
- [Bootstrap count vectors](bootstrap-count-vectors.md)

## ↑ Ancestors (7)

1. [Bootstrapping (statistics)](bootstrapping-statistics.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Bootstrap count vectors](bootstrap-count-vectors.md)
- [Bootstrap failure for a uniform endpoint](bootstrap-failure-for-a-uniform-endpoint.md)
- [Bootstrap sample](bootstrap-sample.md)
- [Bootstrap standard error](bootstrap-standard-error.md)
- [Bootstrap-t confidence interval](bootstrap-t-confidence-interval.md)
- [Bootstrapping (statistics)](bootstrapping-statistics.md)
- [Exact bootstrap distribution for three observations](exact-bootstrap-distribution-for-three-observations.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/24j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-218/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-218/3/d/solution.md)
