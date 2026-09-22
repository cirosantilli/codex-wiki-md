# Conditional bootstrap variance of a sample mean

↑ **Parent:** [Bootstrap sample](bootstrap-sample.md)

Conditionally on the observed values, bootstrap draws are iid from their [empirical distribution](type-information-theory.md). Each draw has [variance](variance-split.md) $n^{-1}\sum_i(a_i-\overline a)^2$, so averaging $n$ independent draws gives the displayed [variance](variance-split.md). The [variance](variance-split.md) across $B$ independent replicate means, using denominator $B-1$, is unbiased for this conditional quantity. Its expectation over the original iid data is $(n-1)\operatorname{Var}(a_1)/n^2$, which is slightly smaller than the actual sampling [variance](variance-split.md) $\operatorname{Var}(a_1)/n$.

## ↑ Ancestors (8)

1. [Bootstrap sample](bootstrap-sample.md)
2. [Bootstrapping (statistics)](bootstrapping-statistics.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Jackknife and bootstrap variance of a sample second moment](jackknife-and-bootstrap-variance-of-a-sample-second-moment.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/4/solution.md)
