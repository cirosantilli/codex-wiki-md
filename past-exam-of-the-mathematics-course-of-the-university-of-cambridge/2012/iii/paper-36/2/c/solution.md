<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Consider any [differentiable-in-quadratic-mean path](../../../../../../differentiability-in-quadratic-mean.md) with [score function](../../../../../../informant-function.md) $g$. Put $\delta_t=\sqrt{f_t}-\sqrt f=(t/2)g\sqrt f+r_t$, where $\|r_t\|_2=o(|t|)$. The [quadratic-mean to L1 density derivative](../../../../../../quadratic-mean-to-l1-density-derivative.md) follows from

$$
f_t-f=2\sqrt f\,\delta_t+\delta_t^2
=tfg+2\sqrt f\,r_t+\delta_t^2.
$$

By the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md),

$$
\|f_t-f-tfg\|_{L^1}
\leq2\|r_t\|_2+\|\delta_t\|_2^2=o(|t|).
$$

Since $a$ is a [bounded function](../../../../../../bounded-function.md), multiplying this [L1 norm](../../../../../../l1-norm.md) bound by $\|a\|_\infty$ proves

$$
\frac{\psi(P_{f_t})-\psi(P_f)}t\longrightarrow P_f(ag)
=P_f\bigl((a-P_fa)g\bigr).
$$

The last equality uses $P_fg=0$. The [derivative](../../../../../../derivative.md) is a [bounded linear functional](../../../../../../continuous-linear-functional.md) of $g\in L^2(P_f)$, so the required [pathwise differentiability of a statistical functional](../../../../../../pathwise-differentiability-of-a-statistical-functional.md) holds, in particular relative to the [statistical tangent set](../../../../../../statistical-tangent-set.md) from part (b). **Its [derivative](../../../../../../derivative.md) is**

$$
\boxed{D\psi_f(g)=P_f[(a-P_fa)g].}
$$

For the explicit [bounded density tilts](../../../../../../bounded-density-tilt.md) in part (b), this [derivative](../../../../../../derivative.md) is also obtained by direct integration, with no remainder term.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
