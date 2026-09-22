<h1 id="18d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Convergence of a numerical method](../../../../../../convergence-of-a-numerical-method.md) on a fixed interval $[0,T]$ means that, as the step size tends to zero and the starting approximations tend to the exact initial values,

$$
\boxed{\max_{0\leq t_n\leq T}|y_n-y(t_n)|\longrightarrow0.}
$$

For a vector-valued [ordinary differential equation](../../../../../../ordinary-differential-equation.md), replace the absolute value by a [norm](../../../../../../norm.md). The interval remains fixed as $h\to0$; a small error at only one step is insufficient.

The [order of a numerical method](../../../../../../order-of-a-numerical-method.md) is measured by its defect on a smooth exact solution. With the unscaled residual convention for a [linear multistep method](../../../../../../linear-multistep-method.md), order at least $p$ means local residual $O(h^{p+1})$; equivalently, the residual divided by $h$ is $O(h^p)$. Order exactly $p$ means the next coefficient does not vanish in general. For a [zero-stable](../../../../../../zero-stability.md) method, under the usual smoothness and [Lipschitz continuity](../../../../../../lipschitz-continuity.md) assumptions and with starting errors $O(h^p)$, this yields [global error](../../../../../../global-discretization-error.md) $O(h^p)$ on the fixed interval. Local order by itself does not imply convergence without stability.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18D](../../18d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
