# Jackknife bias correction

↑ **Parent:** [Statistical inference](statistical-inference-split.md)

For an estimator $T_n$ and leave-one-out versions $T_{(-i)}$, the jackknife bias estimate and corrected estimator are

$$
\widehat B_n=(n-1)\left(\frac1n\sum_iT_{(-i)}-T_n\right),
\qquad
\widetilde T_{\rm JACK}=T_n-\widehat B_n.
$$

If $B_n=a/n+b/n^2+O(n^{-3})$, the correction leaves bias $O(n^{-2})$.

This is the bias-correction application of [Jackknife resampling](jackknife-resampling.md); the same leave-one-out values also yield variance estimates.

**Table of contents**

- [Sample variance](sample-variance.md)
  - [Pooled sample variance](pooled-sample-variance.md)

## ↑ Ancestors (5)

1. [Statistical inference](statistical-inference-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Jackknife resampling](jackknife-resampling.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/28j/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/28k/a/solution.md)
