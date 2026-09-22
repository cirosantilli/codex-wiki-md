<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

Away from $x=\xi$, the [Green function](../../../../../green-s-function.md) solves $G''-G=0$. The solution satisfying the left [boundary condition](../../../../../boundary-condition.md) is proportional to $\sinh x$, while the solution decaying at infinity is proportional to $e^{-x}$. Continuity at $\xi$ and the unit [derivative](../../../../../derivative.md) jump

$$
G_x(\xi+;\xi)-G_x(\xi-;\xi)=1
$$

give

$$
\boxed{
G(x;\xi)=
\begin{cases}
-e^{-\xi}\sinh x,&0<x<\xi,\\
-e^{-x}\sinh\xi,&x>\xi,
\end{cases}
}
$$

or $G=-\sinh(\min\{x,\xi\})e^{-\max\{x,\xi\}}$, the [dirichlet half-line Green function for d2 minus 1](../../../../../dirichlet-half-line-green-function-for-d2-minus-1.md).

The required solution is

$$
y(x)=\int_0^\infty G(x;\xi)e^{-2\xi}\,d\xi.
$$

Evaluation of the two elementary [integrals](../../../../../integral.md), split at $\xi=x$, gives

$$
\boxed{y(x)=\frac13(e^{-2x}-e^{-x})}.
$$

Indeed, direct [differentiation](../../../../../differentiation.md) gives $y''-y=e^{-2x}$, and both [boundary conditions](../../../../../boundary-condition.md) are immediate.

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
