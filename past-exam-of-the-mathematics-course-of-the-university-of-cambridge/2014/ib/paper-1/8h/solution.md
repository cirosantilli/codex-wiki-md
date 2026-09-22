<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

A useful form of the [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) is as follows. For minimization of $f(x)$ subject to $g_j(x)\geq0$ and $h_i(x)=0$, form

$$
L(x,\lambda,\nu)=f(x)-\sum_j\lambda_jg_j(x)+\sum_i\nu_i h_i(x).
$$

If $x_*$ is feasible, $\lambda_j\geq0$, $\lambda_jg_j(x_*)=0$, and $x_*$ globally minimizes $L$ over the ambient domain for these fixed multipliers, then $x_*$ is a global constrained minimizer. Indeed, for every feasible $x$,

$$
f(x)\geq L(x,\lambda,\nu)\geq L(x_*,\lambda,\nu)=f(x_*).
$$

The first inequality uses multiplier signs; the last equality uses feasibility and [complementary slackness](../../../../../complementary-slackness.md). Equality constraints alone require no sign restriction on their multipliers. A stationary point of a differentiable [convex](../../../../../convex-function.md) Lagrangian is a global minimum, which is a common way to verify the theorem's hypothesis.

Here take

$$
L=2x_1^2+2x_2^2+x_3^2-\lambda(x_1+x_2+x_3-1).
$$

Stationarity gives $4x_1=4x_2=2x_3=\lambda$. Feasibility then gives $\lambda=1$ and $x_*=(1/4,1/4,1/2)$. For that multiplier,

$$
L=2(x_1-1/4)^2+2(x_2-1/4)^2+(x_3-1/2)^2+\tfrac12.
$$

The Lagrangian has its unique global minimum at $x_*$, so the sufficiency theorem proves

$$
\boxed{x_*=(1/4,1/4,1/2),\qquad \min f=1/2.}
$$

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
