# Integrated variance of a kernel density estimator

↑ **Parent:** [Kernel density estimation](kernel-density-estimation.md)

For an $L^2$ kernel and an independent sample from a density $f$, the centred [kernel density estimator](kernel-density-estimation.md) has

$$
\mathbb E\|\widehat f_{n,h}-K_h*f\|_2^2=\frac1n\left(\frac{\|K\|_2^2}{h}-\|K_h*f\|_2^2\right).
$$

Independence removes cross terms and [Tonelli theorem](tonelli-theorem.md) integrates the pointwise variance. [Young's convolution inequality](young-s-convolution-inequality.md) ensures $K_h*f\in L^2$ even without $f\in L^2$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) yields the expected-norm bound $\mathbb E\|\widehat f_{n,h}-K_h*f\|_2\le\|K\|_2/\sqrt{nh}$.

**Table of contents**

- [Gaussian autoregressive kernel variance correction](gaussian-autoregressive-kernel-variance-correction.md)

## ↑ Ancestors (9)

1. [Kernel density estimation](kernel-density-estimation.md)
2. [Kernel for density estimation](kernel-for-density-estimation.md)
3. [Density estimation](density-estimation.md)
4. [Nonparametric statistics](nonparametric-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Box-kernel bias of a piecewise constant density](box-kernel-bias-of-a-piecewise-constant-density.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-33/2/solution.md)
- [Second derivative kernel density estimator](second-derivative-kernel-density-estimator.md)
