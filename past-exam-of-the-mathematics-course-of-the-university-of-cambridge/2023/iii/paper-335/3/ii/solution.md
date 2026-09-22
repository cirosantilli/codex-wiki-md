<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $(\sigma_j,u_j,v_j)$ be a [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md), with

$$
Av_j=\sigma_ju_j,
\qquad
A^*u_j=\sigma_jv_j.
$$

The [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) is the generally unbounded map

$$
\boxed{
A^\dagger g
=\sum_j\frac{\langle g,u_j\rangle}{\sigma_j}v_j},
$$

defined when the [Picard criterion](../../../../../../picard-criterion.md) holds, with the component in $\ker A^*$ sent to zero. It is the [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md) of $Af=g$.

A [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md) consists of bounded maps $R_\alpha:Y\to X$ and a parameter rule $α=α(δ,g^{(δ)})$ such that

$$
\alpha\to0,
\qquad
R_\alpha g^{(\delta)}\to A^\dagger g
$$

whenever $\|g^{(\delta)}-g\|\leq\delta$ and $g$ is in the domain of $A^\dagger$.

For [Tikhonov regularization](../../../../../../tikhonov-regularization.md), minimizing

$$
\|Af-g^{(\delta)}\|^2+\alpha\|f\|^2
$$

gives

$$
R_\alpha g^{(\delta)}
=(A^*A+\alpha I)^{-1}A^*g^{(\delta)}
=\sum_j\frac{\sigma_j}{\sigma_j^2+\alpha}
\langle g^{(\delta)},u_j\rangle v_j.
$$

The scalar [spectral filter](../../../../../../spectral-filter.md) satisfies

$$
\sup_{\sigma\geq0}\frac{\sigma}{\sigma^2+\alpha}
=\frac{1}{2\sqrt\alpha},
$$

and consequently

$$
\|R_\alpha(g^{(\delta)}-g)\|
\leq\frac{\delta}{2\sqrt\alpha}.
$$

For exact data, each filter factor $\sigma_j^2/(\sigma_j^2+\alpha)$ tends to one, so $R_\alpha g\to A^\dagger g$. Choosing

$$
\boxed{\alpha(\delta)\to0,
\qquad \frac{\delta}{\sqrt{\alpha(\delta)}}\to0}
$$

therefore makes both the approximation error and propagated data error vanish. For example, $α(δ)=δ$ is an admissible [a priori regularization parameter choice](../../../../../../a-priori-regularization-parameter-choice.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
