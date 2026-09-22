# Beta highest posterior density endpoint characterization

↑ **Parent:** [Highest posterior density interval](highest-posterior-density-interval.md)

For a [beta distribution](beta-distribution.md) with shape parameters $A,B>1$, the [probability density function](probability-density-function.md) vanishes at zero and one and is strictly increasing up to $m=(A-1)/(A+B-2)$ and strictly decreasing afterwards. This follows because the [derivative](derivative.md) of its logarithm is $(A-1)/t-(B-1)/(1-t)$, whose sign changes at $m$.

For each $0<\alpha<1$, the [highest posterior density interval](highest-posterior-density-interval.md) when this [beta distribution](beta-distribution.md) is a [posterior distribution](bayesian-posterior.md) has unique endpoints $0<l<m<u<1$ determined by

$$
F_{A,B}(u)-F_{A,B}(l)=1-\alpha,\qquad
l^{A-1}(1-l)^{B-1}=u^{A-1}(1-u)^{B-1}.
$$

The second equation gives equal endpoint [posterior densities](posterior-density.md). For every density threshold strictly between zero and the modal height there is precisely one crossing on each side. The enclosed [probability](probability.md) is continuous and strictly decreasing from one to zero as the threshold increases, proving existence, uniqueness and the [highest posterior density interval](highest-posterior-density-interval.md) property. The restrictions $A,B>1$ are essential to this two-interior-endpoint characterization; monotone cases use a support boundary instead.

## ↑ Ancestors (8)

1. [Highest posterior density interval](highest-posterior-density-interval.md)
2. [Credible interval](credible-interval.md)
3. [Bayesian statistics](bayesian-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2017/3/b/ii/solution.md)
