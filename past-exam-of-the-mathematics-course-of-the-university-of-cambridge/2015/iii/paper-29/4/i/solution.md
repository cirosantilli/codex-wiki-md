<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A standard form of the [Kakutani solution of the Dirichlet problem](../../../../../../kakutani-solution-of-the-dirichlet-problem.md) uses a bounded [domain](../../../../../../domain-mathematical-analysis.md) $D\subset\mathbb R^d$, continuous [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md) $f\in C(\partial D)$, and regularity of every boundary point for the [Dirichlet problem](../../../../../../dirichlet-problem.md). The boundedness of $D$ makes $\partial D$ a [compact set](../../../../../../compact-space.md), so $f$ is a [bounded function](../../../../../../bounded-function.md) and a [uniformly continuous function](../../../../../../uniformly-continuous-function.md). A bounded domain with $C^2$ boundary is a sufficient geometric case; one must not omit boundary regularity for an arbitrary bounded domain.

One standard analytic characterization of a [regular boundary point](../../../../../../regular-boundary-point.md) on a bounded domain is the existence of a positive harmonic barrier: for each $\xi\in\partial D$ there is a [harmonic function](../../../../../../harmonic-function.md) $h_\xi\in C(\overline D)$ with $h_\xi(\xi)=0$ and $h_\xi(x)>0$ for $x\in\overline D\setminus\{\xi\}$. This is the harmonic form of a [barrier for the Dirichlet problem](../../../../../../barrier-for-the-dirichlet-problem.md); the barrier characterization of regularity is a standard fact of [potential theory](../../../../../../potential-theory.md).

Let $B$ be $d$-dimensional [Brownian motion](../../../../../../brownian-motion-split.md) started at $x\in D$ and let $\tau_D=\inf\{t\geq0:B_t\notin D\}$ be its [Brownian exit time](../../../../../../brownian-exit-time.md). Then the unique solution in $C(\overline D)\cap C^2(D)$ is

$$
\boxed{u(x)=\mathbb E_x[f(B_{\tau_D})]\quad(x\in D),\qquad u(\xi)=f(\xi)\quad(\xi\in\partial D).}
$$

Equivalently, $u(x)=\int_{\partial D}f(\xi)\,\omega_D(x,d\xi)$, where $\omega_D$ is [harmonic measure](../../../../../../harmonic-measure.md), the exit [probability distribution](../../../../../../probability-distribution.md) of [Brownian motion](../../../../../../brownian-motion-split.md). The [harmonic function](../../../../../../harmonic-function.md) equation is $\Delta u=0$, with the [Laplace operator](../../../../../../laplace-operator.md) convention $\Delta=\sum_j\partial_j^2$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
