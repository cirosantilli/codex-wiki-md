<h1 id="nadaraya-watson-estimator">Nadaraya–Watson estimator</h1>

↑ **Parent:** [Local polynomial regression](local-polynomial-regression.md)

This local-constant estimator is one particular [kernel regression](kernel-regression.md) method.

The Nadaraya–Watson estimator is the degree-zero local polynomial estimate

$$
\widehat m(x)=
\frac{\sum_iK((x_i-x)/h)Y_i}
{\sum_iK((x_i-x)/h)}.
$$

At a support boundary it generally has first-order bias because it reproduces constants but not linear functions.

**Table of contents**

- [Interior absolute-error rate of the Nadaraya-Watson estimator](interior-absolute-error-rate-of-the-nadaraya-watson-estimator.md)
- [Boundary bias of local constant regression](boundary-bias-of-local-constant-regression.md)
  - [Second-order boundary expansion for local constant regression](second-order-boundary-expansion-for-local-constant-regression.md)
- [Mean absolute error of local constant regression](mean-absolute-error-of-local-constant-regression.md)
- [Interior first-order bias cancellation for local constant regression](interior-first-order-bias-cancellation-for-local-constant-regression.md)

## ↑ Ancestors (8)

1. [Local polynomial regression](local-polynomial-regression.md)
2. [Nonparametric regression](nonparametric-regression.md)
3. [Nonparametric statistics](nonparametric-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Kernel regression](kernel-regression.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-210/3/solution.md)
- [Uniform smoothing kernel](uniform-smoothing-kernel.md)
