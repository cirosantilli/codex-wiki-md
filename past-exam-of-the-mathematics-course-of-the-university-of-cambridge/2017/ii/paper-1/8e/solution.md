<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

Assume the [holonomic constraints](../../../../../holonomic-constraint.md) have [linearly independent](../../../../../linear-independence.md) [gradients](../../../../../gradient.md), so their common level [set](../../../../../set-split.md) is locally a smooth constraint [manifold](../../../../../topological-manifold.md) parametrized by $q_1,\ldots,q_n$. The multiplier form of the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) is

$$
\frac d{dt}L_{\dot x_A}-L_{x_A}
=\sum_\alpha\lambda_\alpha\partial_A f_\alpha.
$$

At fixed time $\sum_A\partial_A f_\alpha\,\partial_i x_A=0$. The [chain rule](../../../../../chain-rule.md) for the reduced [Lagrangian](../../../../../lagrangian.md) gives

$$
\frac d{dt}\mathcal L_{\dot q_i}-\mathcal L_{q_i}
=\sum_A\left(\frac d{dt}L_{\dot x_A}-L_{x_A}\right)\partial_i x_A=0.
$$

Conversely, if these reduced equations hold, the Cartesian Euler-Lagrange residual annihilates every tangent direction. [Linear independence](../../../../../linear-independence.md) of the constraint [gradients](../../../../../gradient.md) implies that it is a linear combination of those [gradients](../../../../../gradient.md), giving the required [Lagrange multipliers](../../../../../lagrange-multiplier.md). This proves the local equivalence, including time-dependent constraints; singular constraints would need separate analysis.

For the bead, $\dot y=f'(x)\dot x$, so

$$
\boxed{\mathcal L=\frac12(1+f'(x)^2)\dot x^2},\qquad
(1+f'^2)\ddot x+f'f''\dot x^2=0.
$$

The autonomous [conservation of energy](../../../../../conservation-of-energy.md) gives $E=\tfrac12(1+f'^2)\dot x^2$. If $E>0$, the motion has a fixed sign $s=\operatorname{sgn}\dot x$ and

$$
\boxed{t=t_*+\frac{s}{\sqrt{2E}}\int_{x_*}^{x}\sqrt{1+f'(u)^2}\,du}.
$$

The [integral](../../../../../integral.md) is the signed [arc length](../../../../../arc-length.md) divided by the constant speed, and is locally invertible. The special solution $E=0$ is a stationary bead, for which writing time as a [function](../../../../../function-split.md) of its unchanging position is not meaningful.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
