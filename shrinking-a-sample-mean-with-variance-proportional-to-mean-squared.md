# Shrinking a sample mean with variance proportional to mean squared

↑ **Parent:** [Mean squared error](mean-squared-error.md)

If independent observations have mean $\theta$ and variance $\theta^2$, the scaled [sample mean](sample-mean.md) has

$$
\operatorname{MSE}(k\bar X)=\theta^2[(k-1)^2+k^2/n].
$$

For $\theta\ne0$, it improves on the unbiased sample mean precisely when $(n-1)/(n+1)<k<1$. The optimal scale is $k=n/(n+1)$ and its risk is $\theta^2/(n+1)$. At $\theta=0$ all risks vanish and strict improvement is impossible.

## ↑ Ancestors (8)

1. [Mean squared error](mean-squared-error.md)
2. [Risk function](risk-function.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/7h/ii/solution.md)
