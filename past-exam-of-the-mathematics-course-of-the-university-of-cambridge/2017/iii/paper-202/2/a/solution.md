<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [polarization identity](../../../../../../polarization-identity.md) of the [quadratic variations](../../../../../../quadratic-variation.md):

$$
\boxed{[M,N]=\frac14\bigl([M+N]-[M-N]\bigr).}
$$

This is continuous and adapted, starts at zero, and has [finite variation](../../../../../../total-variation-of-a-function.md) on every compact interval because it is a difference of two nondecreasing processes. The defining [quadratic variation](../../../../../../quadratic-variation.md) property gives that $(M+N)^2-[M+N]$ and $(M-N)^2-[M-N]$ are [continuous local martingales](../../../../../../continuous-local-martingale.md); their difference divided by four is $MN-[M,N]$. This proves existence without assuming a product formula involving an as yet undefined [quadratic covariation](../../../../../../quadratic-covariation.md).

If $C$ and $D$ both satisfy the requirements, $C-D$ is a continuous [finite-variation process](../../../../../../finite-variation-process.md) and a [local martingale](../../../../../../local-martingale.md). By [continuous finite-variation local martingale is constant](../../../../../../continuous-finite-variation-local-martingale-is-constant.md), it is constant; its initial value is zero, so $C=D$ up to [indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md).

There is a minor initial-value convention in this characterization. The displayed uncentred [local martingale](../../../../../../local-martingale.md) identity is directly valid when $M_0=N_0=0$, or when the initial terms have the requisite integrability. With arbitrary finite initial values, centre the [quadratic variation](../../../../../../quadratic-variation.md) construction and use $MN-M_0N_0-[M,N]$, which starts at zero. Adding back $M_0N_0$ requires it to be integrable under the usual definition of a [local martingale](../../../../../../local-martingale.md); the [quadratic covariation](../../../../../../quadratic-covariation.md) itself is unaffected by centring.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
