<h1 id="2/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Starting from zero, the [Landweber iteration](../../../../../../../landweber-iteration.md) is

$$
\boxed{u_\delta^{(0)}=0,\qquad
u_\delta^{(k+1)}=u_\delta^{(k)}+\tau K^*(f^\delta-Ku_\delta^{(k)}).}
$$

For $K\neq0$, take the [step size](../../../../../../../step-size.md) $0<\tau<2/\|K\|^2$. Iterating the linear update gives

$$
R_{1/k}=\tau\sum_{m=0}^{k-1}(I-\tau K^*K)^mK^*,
$$

and its [Landweber spectral filter](../../../../../../../landweber-spectral-filter.md) in a [singular system of a compact operator](../../../../../../../singular-system-of-a-compact-operator.md) is

$$
\boxed{R_{1/k}f^\delta=
\sum_j\frac{1-(1-\tau\sigma_j^2)^k}{\sigma_j}
\langle f^\delta,w_j\rangle v_j.}
$$

The strict upper [step size](../../../../../../../step-size.md) bound makes $|1-\tau\sigma_j^2|<1$ for every positive [singular value](../../../../../../../singular-value.md). A common more restrictive choice is $0<\tau\leq\|K\|^{-2}$, giving nonnegative damping factors. Each finite iterate is bounded and linear; [early stopping of Landweber iteration](../../../../../../../early-stopping-of-landweber-iteration.md) controls the amplification of noise as smaller [singular values](../../../../../../../singular-value.md) are progressively inverted. If $K=0$, every iterate is zero for any positive [step size](../../../../../../../step-size.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
