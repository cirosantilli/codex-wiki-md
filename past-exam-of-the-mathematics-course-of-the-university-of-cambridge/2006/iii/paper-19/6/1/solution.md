<h1 id="6/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The printed identity has a sign error. With the defined [Kostant partition function](../../../../../../kostant-partition-function.md) and the exponent $e^{-\nu}$, the cancelling factors must be $1-e^{-\alpha}$. This is already visible for $SU(2)$ with [positive root](../../../../../../positive-root.md) $\alpha$: the formal series $\sum_{k\geq0}e^{-k\alpha}$ multiplied by $1-e^\alpha$ is $-e^\alpha$, not $1$.

For the corrected formula, a partition of $\nu$ is a tuple of [nonnegative integers](../../../../../../natural-number.md) $(k_\alpha)_{\alpha>0}$ satisfying $\nu=\sum_{\alpha>0}k_\alpha\alpha$. The order of summands is not counted. Multiplying the formal [geometric series](../../../../../../geometric-series.md) yields

$$
\prod_{\alpha>0}\left(\sum_{k\geq0}e^{-k\alpha}\right)
=\sum_\nu p(\nu)e^{-\nu}.
$$

This product is coefficientwise meaningful. Choose a [linear functional](../../../../../../linear-functional.md) strictly positive on every [positive root](../../../../../../positive-root.md). For a fixed $\nu$ it bounds each $k_\alpha$, so only finitely many tuples contribute. We are working in the completion supported on the negative positive-root cone, not claiming convergence of an ordinary [Fourier series](../../../../../../fourier-series-split.md) on the [torus](../../../../../../torus.md).

Each [geometric series](../../../../../../geometric-series.md) cancels its factor $1-e^{-\alpha}$, proving

$$
\boxed{\left(\sum_\nu p(\nu)e^{-\nu}\right)\prod_{\alpha>0}(1-e^{-\alpha})=1.}
$$

Equivalently, reversing all the exponential signs gives $(\sum_\nu p(\nu)e^{\nu})\prod_{\alpha>0}(1-e^\alpha)=1$ in the opposite completion. More generally, if $N$ is the number of [positive roots](../../../../../../positive-root.md), the expression literally printed in the paper equals

$$
(-1)^N e^{2\rho},
$$

since $\prod_{\alpha>0}(1-e^\alpha)=(-1)^N e^{2\rho}\prod_{\alpha>0}(1-e^{-\alpha})$. Thus the correction is substantive, not merely a choice of Fourier convention.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [6](../../6.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
