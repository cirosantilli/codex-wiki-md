<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $u(x,t)=U(\xi,\eta)$, where $\xi=x-t$ and $\eta=x+t$. The [chain rule](../../../../../../chain-rule.md) gives

$$
\partial_x=\partial_\xi+\partial_\eta,\qquad
\partial_t=-\partial_\xi+\partial_\eta.
$$

For a twice continuously differentiable [classical solution](../../../../../../classical-solution.md), mixed [partial derivatives](../../../../../../partial-derivative.md) commute, so the [wave equation](../../../../../../wave-equation-split.md) becomes

$$
0=u_{tt}-u_{xx}=-4U_{\xi\eta}.
$$

Hence $U_\xi$ depends only on $\xi$. Integrating first in $\xi$ yields the [countertravelling decomposition of the one-dimensional wave equation](../../../../../../countertravelling-decomposition-of-the-one-dimensional-wave-equation.md):

$$
\boxed{u(x,t)=F(x-t)+G(x+t).}
$$

On a rectangular domain in $(\xi,\eta)$ this follows immediately; on the full line for $t\geq0$, the connected characteristic slices give the same representation. The two terms travel at [wave speed](../../../../../../wave-speed.md) one in opposite directions.

Impose the [initial conditions](../../../../../../initial-condition.md). At $t=0$,

$$
F(x)+G(x)=f(x),\qquad -F'(x)+G'(x)=g(x).
$$

Differentiate the first identity and combine:

$$
F'(x)=\frac{f'(x)-g(x)}2,\qquad G'(x)=\frac{f'(x)+g(x)}2.
$$

If $H(x)=\int_{x_*}^xg(s)\,ds$, then $F=(f-H)/2+C$ and $G=(f+H)/2-C$. Substitution cancels $C$ and the arbitrary base point $x_*$, giving [D'Alembert's formula](../../../../../../d-alembert-s-formula.md):

$$
\boxed{u(x,t)=\frac{f(x-t)+f(x+t)}2+\frac12\int_{x-t}^{x+t}g(s)\,ds.}
$$

For example, $f\in C^2$ and $g\in C^1$ make this a [classical solution](../../../../../../classical-solution.md) of the [wave equation](../../../../../../wave-equation-split.md) satisfying both [initial conditions](../../../../../../initial-condition.md). The same formula defines a [weak solution](../../../../../../weak-solution.md) for less regular data, including the continuous piecewise smooth data of part (b).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
