# Jackknife and bootstrap variance of a sample second moment

↑ **Parent:** [Jackknife variance estimator](jackknife-variance-estimator.md)

For independent identically distributed observations with finite fourth [moment](moment.md), the [sample mean](sample-mean.md) of their squares has [sampling variance](variance-of-an-estimator.md) $\operatorname{Var}(X^2)/n$. Its [Jackknife variance estimator](jackknife-variance-estimator.md) is exactly the displayed unbiased estimator, since its leave-one-out values differ from their average by $-(x_i^2-\overline{x^2})/(n-1)$. The [conditional bootstrap variance of a sample mean](conditional-bootstrap-variance-of-a-sample-mean.md) is $\widehat v_B=n^{-2}\sum_i(x_i^2-\overline{x^2})^2=(n-1)\widehat v_J/n$. Thus the two methods have a known finite-sample scaling difference, despite sharing the same large-sample target.

## ↑ Ancestors (7)

1. [Jackknife variance estimator](jackknife-variance-estimator.md)
2. [Jackknife resampling](jackknife-resampling.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/4/solution.md)
