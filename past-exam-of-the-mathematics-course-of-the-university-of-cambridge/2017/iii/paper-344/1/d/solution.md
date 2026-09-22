<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The post-[quench](../../../../../../quench-statistical-physics.md) [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md) has $r_1(q)=\Gamma(a_1+\kappa q^2)$. Its future noise is independent of the initial field. Consequently the cross term between the initial [Fourier mode](../../../../../../fourier-mode.md) and its future noise integral has zero expectation. The [Itô isometry](../../../../../../ito-isometry.md), or the given white-noise covariance, then yields

$$
\begin{aligned}
S_q(t)&=e^{-2r_1(q)t}S_q(0)+2\Gamma k_BT\int_0^t e^{-2r_1(q)(t-s)}\,ds\\
&=e^{-2r_1(q)t}S_q(0)+\frac{k_BT}{a_1+\kappa q^2}\left[1-e^{-2r_1(q)t}\right].
\end{aligned}
$$

The initial Gaussian [Boltzmann distribution](../../../../../../boltzmann-distribution.md), with $a=a_0$, gives $S_q(0)=k_BT/(a_0+\kappa q^2)$ in the same unitary normalization. Thus the [Gaussian Model A quench](../../../../../../gaussian-model-a-quench.md) has

$$
\boxed{S_q(t)=\frac{k_BT}{a_1+\kappa q^2}+\left[\frac{k_BT}{a_0+\kappa q^2}-\frac{k_BT}{a_1+\kappa q^2}\right]e^{-2\Gamma(a_1+\kappa q^2)t}.}
$$

The [static structure factor](../../../../../../static-structure-factor.md) interpolates monotonically mode by mode between its two positive equilibrium values. The covariance relaxes at twice the amplitude decay rate. These statements assume that $T$, $\Gamma$ and $\kappa$ are unchanged by the quench; both $a_0,a_1>0$ exclude a spinodal instability.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
