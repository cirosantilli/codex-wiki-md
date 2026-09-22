<h1 id="37b/solution">Solution</h1>

↑ **Parent:** [37B](../37b.md)

For isentropic gas with $P=K\rho^\gamma$, $\gamma>1$, the [sound speed](../../../../../speed-of-sound.md) obeys $c^2=P'(\rho)$. The one-dimensional mass and momentum equations are

$$
\rho_t+u\rho_x+\rho u_x=0,\qquad u_t+uu_x+\frac{c^2}{\rho}\rho_x=0.
$$

Since $c\propto\rho^{(\gamma-1)/2}$, these imply

$$
c_t+uc_x+\frac{\gamma-1}2cu_x=0,\qquad
u_t+uu_x+\frac2{\gamma-1}cc_x=0.
$$

Adding and subtracting yields the [Riemann invariants](../../../../../riemann-invariant.md)

$$
\boxed{R_\pm=u\pm\frac{2(c-c_0)}{\gamma-1},\qquad
(\partial_t+(u\pm c)\partial_x)R_\pm=0.}
$$

A [simple wave](../../../../../simple-wave.md) has one invariant constant throughout. For a right-moving wave into a resting state with [sound speed](../../../../../speed-of-sound.md) $c_0$, $R_-=0$, so $c=c_0+(\gamma-1)u/2$ and the right characteristic speed is $c_0+bu$, $\boxed{b=(\gamma+1)/2}$.

For the damped scalar equation, characteristics from $\xi$ satisfy

$$
\boxed{u=e^{-\alpha t}u_0(\xi),\qquad
x=c_0t+\xi+\frac b\alpha(1-e^{-\alpha t})u_0(\xi).}
$$

Assume smooth bounded initial data with bounded [derivative](../../../../../derivative.md), and the stated maximal compressive slope exists. Then

$$
J=\frac{\partial x}{\partial\xi}=1+\frac b\alpha(1-e^{-\alpha t})u_0'(\xi),\qquad
u_x=\frac{e^{-\alpha t}u_0'(\xi)}J.
$$

For the [damping threshold for a simple wave](../../../../../damping-threshold-for-a-simple-wave.md), if $m=\max_\xi[-u_0'(\xi)]>0$, put $\boxed{\alpha_c=bm}$. For $0<\alpha<\alpha_c$, a [gradient blow-up](../../../../../gradient-blow-up.md) first occurs at

$$
\boxed{t_s=-\frac1\alpha\log\left(1-\frac\alpha{\alpha_c}\right).}
$$

For $\alpha>\alpha_c$, $J$ stays uniformly positive. At $\alpha=\alpha_c$ it still satisfies $J\geq e^{-\alpha t}>0$ for every finite time. At a point attaining the minimum slope, $u_x=u_0'$ for all time, rather than blowing up. Hence the precise conclusion is **no finite-time shock occurs when $\alpha\geq\alpha_c$**, not the printed strict “if and only if $\alpha>\alpha_c$”. Equality only makes the limiting characteristic map degenerate as $t\to\infty$. The profile $u_0(\xi)=-\sin\xi$ directly verifies this endpoint distinction. If there is no compressive slope, take $\alpha_c=0$; no finite-time shock occurs for positive damping. A nonattained maximal slope is interpreted with a supremum and the corresponding infimum of breakdown times. The gas interpretation also requires $c_0+(\gamma-1)u/2>0$.

## ↑ Ancestors (10)

1. [37B](../37b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
