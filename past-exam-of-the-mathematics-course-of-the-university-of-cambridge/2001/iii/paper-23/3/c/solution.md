<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [Itô process](../../../../../../ito-process.md) $dX_t=a_tdt+b_tdW_t$ and $F\in C^{1,2}$, the differential [Itô formula](../../../../../../ito-s-lemma.md) is

$$
\boxed{dF(t,X_t)=\left(F_t+a_tF_x+\frac12b_t^2F_{xx}\right)dt+b_tF_x\,dW_t,}
$$

where the [derivatives](../../../../../../derivative.md) are evaluated at $(t,X_t)$. A multidimensional version replaces $b_t^2F_{xx}$ by the contraction of the [Itô diffusion](../../../../../../ito-diffusion.md) [covariance matrix](../../../../../../covariance-matrix.md) with the spatial [Hessian](../../../../../../hessian-matrix.md).

For a heuristic derivation, partition time and use the Euler increment $\Delta X=a\,\Delta t+b\sqrt{\Delta t}\,Z$, where $Z$ is standard normal. A second-order [Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
\Delta F=F_t\Delta t+F_x\Delta X+\frac12F_{xx}(\Delta X)^2+\text{higher-order terms}.
$$

The term $b^2(\Delta W)^2$ has order $\Delta t$, so it survives summation; ordinary first-order calculus would incorrectly discard it. For independent [Brownian motion](../../../../../../brownian-motion-split.md) increments,

$$
\mathbb E\sum_k[(\Delta W_k)^2-\Delta t_k]=0,\qquad
\operatorname{Var}\left(\sum_k[(\Delta W_k)^2-\Delta t_k]\right)
=2\sum_k(\Delta t_k)^2\longrightarrow0.
$$

This gives the [quadratic variation](../../../../../../quadratic-variation.md) $[W]_t=t$. The summed mixed $dt\,dW$ terms and $dt^2$ terms vanish, while the linear random increments converge to an [Itô integral](../../../../../../ito-integral.md). After localizing bounded coefficients and [derivatives](../../../../../../derivative.md), Taylor remainders are negligible and the surviving terms give the formula. Thus $(dW)^2=dt$ is shorthand for a statement about summed [quadratic variation](../../../../../../quadratic-variation.md), not an equality of individual random increments.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
