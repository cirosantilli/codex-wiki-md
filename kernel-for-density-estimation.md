# Kernel for density estimation

↑ **Parent:** [Density estimation](density-estimation.md)

A kernel for [density estimation](density-estimation.md) is an [integrable function](lebesgue-integrable-function.md) $K:\mathbb R\to\mathbb R$ with unit [integral](integral.md). For an ordinary [kernel density estimator](kernel-density-estimation.md) that is itself a [probability density function](probability-density-function.md), take

$$
K(u)\geq0,\qquad \int_{\mathbb R}K(u)\,du=1,\qquad K_h(u)=\frac1hK\!\left(\frac uh\right),\quad h>0.
$$

Thus $K$ specifies the bump's shape and the [smoothing bandwidth](smoothing-bandwidth.md) $h$ specifies its width. The factor $1/h$ preserves area: doubling the [smoothing bandwidth](smoothing-bandwidth.md) doubles the width and halves the height. An [even function](even-function.md) $K(u)=K(-u)$ is a common choice; when its absolute first [moment](moment.md) is finite, its [mean](expected-value.md) is zero. Symmetry is useful but is not required for normalization.

The [Gaussian density kernel](gaussian-density-kernel.md) is the [standard normal density](standard-normal-density.md), $K(u)=(2\pi)^{-1/2}e^{-u^2/2}$. Its rescaled translate $K_h(x-X_i)$ is the [normal probability density](normal-density.md) with [mean](expected-value.md) $X_i$ and [standard deviation](standard-deviation.md) $h$. It is positive everywhere, whereas an [Epanechnikov kernel](epanechnikov-kernel.md) has [compact support](compact-support.md). With the [Gaussian density kernel](gaussian-density-kernel.md), the [smoothing bandwidth](smoothing-bandwidth.md) is a [standard deviation](standard-deviation.md), not a cutoff beyond which observations have no influence.

The broader convention also allows signed [kernels of order ell](kernel-of-order-ell.md), such as the [flat-top kernel for density estimation](flat-top-kernel-for-density-estimation.md), to cancel [moments](moment.md) and reduce the [bias of an estimator](bias-of-an-estimator.md). Their unit [integral](integral.md) still normalizes total area, but a resulting [kernel density estimator](kernel-density-estimation.md) can take negative values and need not be a [probability density function](probability-density-function.md). Nonnegativity is therefore an additional condition, not a consequence of unit [integral](integral.md).

**Table of contents**

- [Triweight kernel](triweight-kernel.md)
  - [Triweight density minimizes integrated squared curvature](triweight-density-minimizes-integrated-squared-curvature.md)
- [Gaussian density kernel](gaussian-density-kernel.md)
- [Epanechnikov kernel](epanechnikov-kernel.md)
  - [Optimality of the Epanechnikov kernel](optimality-of-the-epanechnikov-kernel.md)
- [Flat-top kernel for density estimation](flat-top-kernel-for-density-estimation.md)
  - [Parametric-rate kernel estimation of a bandlimited density](parametric-rate-kernel-estimation-of-a-bandlimited-density.md)
- [Kernel of order ell](kernel-of-order-ell.md)
  - [Legendre polynomial kernel construction](legendre-polynomial-kernel-construction.md)
- [Kernel density estimation](kernel-density-estimation.md)
  - [Gaussian kernel density worked example](gaussian-kernel-density-worked-example.md)
  - [History of kernel density estimation](history-of-kernel-density-estimation.md)
  - [Exact mean integrated squared error of a kernel density estimator](exact-mean-integrated-squared-error-of-a-kernel-density-estimator.md)
  - [Pointwise optimal kernel bandwidth](pointwise-optimal-kernel-bandwidth.md)
    - [Normal-density local-to-global bandwidth ratio](normal-density-local-to-global-bandwidth-ratio.md)
  - [Canonical kernel for density estimation](canonical-kernel-for-density-estimation.md)
  - [Pointwise central limit theorem for a kernel density estimator](pointwise-central-limit-theorem-for-a-kernel-density-estimator.md)
  - [Third-order pointwise kernel error bound](third-order-pointwise-kernel-error-bound.md)
  - [Integrated variance of a kernel density estimator](integrated-variance-of-a-kernel-density-estimator.md)
    - [Gaussian autoregressive kernel variance correction](gaussian-autoregressive-kernel-variance-correction.md)
  - [Pointwise minimax rate for Hölder density estimation](pointwise-minimax-rate-for-holder-density-estimation.md)
  - [Bias of a kernel density estimator](bias-of-a-kernel-density-estimator.md)
    - [Boundary bias of a kernel density estimator](boundary-bias-of-a-kernel-density-estimator.md)
    - [Integrated second-order kernel bias bound](integrated-second-order-kernel-bias-bound.md)
    - [Integrated squared bias from a density jump](integrated-squared-bias-from-a-density-jump.md)
      - [Box-kernel bias of a piecewise constant density](box-kernel-bias-of-a-piecewise-constant-density.md)
    - [Second-order pointwise bias bound for kernel density estimation](second-order-pointwise-bias-bound-for-kernel-density-estimation.md)
  - [Lepski bandwidth selection method](lepski-bandwidth-selection-method.md)
  - [Derivative kernel density estimator](derivative-kernel-density-estimator.md)
    - [Second derivative kernel density estimator](second-derivative-kernel-density-estimator.md)
      - [Integrated squared density curvature](integrated-squared-density-curvature.md)
        - [Scale-invariant density curvature](scale-invariant-density-curvature.md)
    - [Nikolsky class](nikolsky-class.md)
    - [MISE rate for derivative kernel density estimation](mise-rate-for-derivative-kernel-density-estimation.md)

## ↑ Ancestors (7)

1. [Density estimation](density-estimation.md)
2. [Nonparametric statistics](nonparametric-statistics-split.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Boundary bias of a kernel density estimator](boundary-bias-of-a-kernel-density-estimator.md)
- [Canonical kernel for density estimation](canonical-kernel-for-density-estimation.md)
- [Epanechnikov kernel](epanechnikov-kernel.md)
- [Flat-top kernel for density estimation](flat-top-kernel-for-density-estimation.md)
- [Gaussian density kernel](gaussian-density-kernel.md)
- [Integrated second-order kernel bias bound](integrated-second-order-kernel-bias-bound.md)
- [Interior absolute-error rate of the Nadaraya-Watson estimator](interior-absolute-error-rate-of-the-nadaraya-watson-estimator.md)
- [Kernel density estimation](kernel-density-estimation.md)
- [Kernel of a U-statistic](kernel-of-a-u-statistic.md)
- [Legendre polynomial kernel construction](legendre-polynomial-kernel-construction.md)
- [Nonparametric statistics](nonparametric-statistics-split.md)
- [Optimality of the Epanechnikov kernel](optimality-of-the-epanechnikov-kernel.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-42/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-42/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-210/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-210/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-210/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-210/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-210/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-210/2/solution.md)
- [Pointwise central limit theorem for a kernel density estimator](pointwise-central-limit-theorem-for-a-kernel-density-estimator.md)
- [Second-order pointwise bias bound for kernel density estimation](second-order-pointwise-bias-bound-for-kernel-density-estimation.md)
- [Smoothing bandwidth](smoothing-bandwidth.md)
- [Third-order pointwise kernel error bound](third-order-pointwise-kernel-error-bound.md)
