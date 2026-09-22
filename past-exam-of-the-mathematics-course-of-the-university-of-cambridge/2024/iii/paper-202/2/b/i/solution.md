<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Apply the [realized absolute covariation](../../../../../../../realized-absolute-covariation.md) theorem to each dyadic [partition of an interval](../../../../../../../partition-of-an-interval.md). More explicitly, use the continuous increasing clock $C=[M]+[N]$ and the [Radon-Nikodym theorem](../../../../../../../radon-nikodym-theorem.md) to write

$$
a=\frac{d[M]}{dC},\qquad b=\frac{d[N]}{dC},\qquad c=\frac{d[M,N]}{dC}.
$$

For each time, let $(U,V)$ have the centered [bivariate normal distribution](../../../../../../../bivariate-normal-distribution.md) with covariance matrix $\left(\begin{smallmatrix}a&c\\c&b\end{smallmatrix}\right)$, and define

$$
\widetilde V_t=\int_0^t\mathbb E|UV|\,dC.
$$

This process is continuous and increasing. To prove convergence, localize $M,N$, represent the pair as [stochastic integrals](../../../../../../../stochastic-integral.md) against a two-dimensional [Brownian motion](../../../../../../../brownian-motion-split.md), and approximate the integrands in $L^2(dC)$ by bounded step [previsible processes](../../../../../../../predictable-process.md). For step integrands, the result is the [weak law of large numbers](../../../../../../../weak-law-of-large-numbers.md) applied on each block to independent [Gaussian random variables](../../../../../../../gaussian-random-variable.md). The [Burkholder-Davis-Gundy inequality](../../../../../../../burkholder-davis-gundy-inequalities.md) and the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) make the error uniform on each compact interval in probability. Consequently

$$
\widetilde V^n\longrightarrow\widetilde V
$$

in the sense of [uniform convergence on compacts in probability](../../../../../../../uniform-convergence-on-compacts-in-probability.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
