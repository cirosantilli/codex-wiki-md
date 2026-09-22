<h1 id="38b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $H=\dot a/a$. The nonzero Christoffel symbols for the flat FLRW metric are

$$
\Gamma^t_{ij}=a\dot a\,\delta_{ij},
\qquad
\Gamma^i_{tj}=\Gamma^i_{jt}=H\delta^i_j.
$$

The mixed Einstein tensor is

$$
G_t{}^t=-3H^2,\qquad
G_i{}^j=-\left(2\frac{\ddot a}{a}+H^2\right)\delta_i^j.
$$

For a mixed tensor,

$$
\nabla_\nu G_\mu{}^\nu
=\partial_\nu G_\mu{}^\nu
+\Gamma^\nu_{\nu\lambda}G_\mu{}^\lambda
-\Gamma^\lambda_{\nu\mu}G_\lambda{}^\nu.
$$

For $\mu=t$, direct substitution gives

$$
\begin{aligned}
\nabla_\nu G_t{}^\nu
&=\frac d{dt}(-3H^2)+3H(-3H^2)
-3H\left[-\left(2\frac{\ddot a}{a}+H^2\right)\right]\\
&=-6H\left(\dot H+H^2-\frac{\ddot a}{a}\right)=0.
\end{aligned}
$$

For each spatial $\mu$, homogeneity makes the [partial derivatives](../../../../../../partial-derivative.md) vanish and the remaining diagonal connection terms cancel pairwise. This verifies the [flat FLRW Einstein-tensor divergence](../../../../../../flat-flrw-einstein-tensor-divergence.md) directly.

In vacuum,

$$
G_\mu{}^\nu+\Lambda\delta_\mu^\nu=0.
$$

The $tt$ equation is

$$
H^2=\frac{\Lambda}{3}.
$$

Choosing the positive root gives the expanding [de Sitter scale factor in flat slicing](../../../../../../de-sitter-scale-factor-in-flat-slicing.md)

$$
\boxed{a(t)=a_0\exp\!\left(\sqrt{\frac{\Lambda}{3}}\,t\right)},
$$

and the spatial equation is then automatically satisfied.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38B](../../38b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
