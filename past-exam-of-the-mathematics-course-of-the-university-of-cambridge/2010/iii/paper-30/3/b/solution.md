<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [link-route incidence matrix](../../../../../../link-route-incidence-matrix.md) $A$, the [reduced-load approximation](../../../../../../reduced-load-approximation.md) and [Erlang loss formula](../../../../../../erlang-loss-formula.md) give

$$
\boxed{B_j=E(a_j,C_j),\qquad a_j=\sum_r A_{jr}\nu_r\prod_{k\ne j}(1-B_k)^{A_{kr}}.}
$$

Introduce $y_j=-\log(1-B_j)$ and accepted route flows $x_r=\nu_r e^{-(A^Ty)_r}$. Multiplying the reduced load by the link's own acceptance probability gives

$$
a_j(1-B_j)=\sum_r A_{jr}x_r=U(y_j,C_j).
$$

These are precisely the [first-order optimality conditions](../../../../../../first-order-optimality-condition.md) for the [convex potential for the Erlang fixed point](../../../../../../convex-potential-for-the-erlang-fixed-point.md), since

$$
\frac{\partial F}{\partial y_j}=-\sum_r A_{jr}\nu_r e^{-(A^Ty)_r}+U(y_j,C_j).
$$

Each exponential term is a [convex function](../../../../../../convex-function.md), and the integral of the strictly increasing function $U(\cdot,C_j)$ is a [strictly convex function](../../../../../../strictly-convex-function.md). Hence $F$ is a [strictly convex function](../../../../../../strictly-convex-function.md). Moreover $U(z,C_j)\to C_j>0$ as $z\to\infty$, by the saturation of the [carried load of an Erlang loss resource](../../../../../../carried-load-of-an-erlang-loss-resource.md). Its integrals tend to infinity at least linearly, so $F$ is a [coercive function](../../../../../../coercive-function.md) on the nonnegative orthant and has a unique minimizer.

At $y_j=0$, $U(0,C_j)=0$. If link $j$ is used by any positive-rate route, then $\partial_jF<0$, excluding a boundary minimizer there. An unused link instead minimizes at $y_j=0$ and has zero derivative. Thus the minimizer satisfies the displayed flow equations for every link. Conversely, those equations imply $\nabla F=0$ and therefore minimize the [convex potential for the Erlang fixed point](../../../../../../convex-potential-for-the-erlang-fixed-point.md). Finally $U(y,C)=a[1-E(a,C)]$ with $y=-\log(1-E(a,C))$ converts the flow equations back to $B_j=E(a_j,C_j)$. **The Erlang fixed point approximation has exactly one solution under fixed routing.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
