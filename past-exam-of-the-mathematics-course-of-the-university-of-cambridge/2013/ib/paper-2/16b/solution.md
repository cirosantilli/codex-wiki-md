<h1 id="16b/solution">Solution</h1>

↑ **Parent:** [16B](../16b.md)

For the [Dirichlet Green's function](../../../../../dirichlet-green-function.md), solve $-DG_{xx}=\delta(x-\xi)$ with zero endpoint values. Away from $\xi$, $G$ is linear. Continuity at $\xi$ and the [derivative](../../../../../derivative.md) jump $G_x(\xi+,\xi)-G_x(\xi-,\xi)=-1/D$ give

$$
\boxed{G(x,\xi)=\begin{cases}\dfrac{x(l-\xi)}{Dl},&x\leq\xi,\\[4pt]\dfrac{\xi(l-x)}{Dl},&x\geq\xi.\end{cases}}
$$

For nonzero [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), subtract their linear interpolant. The resulting [boundary value problem](../../../../../boundary-value-problem.md) has solution

$$
\boxed{u(x)=\alpha+\frac{\beta-\alpha}{l}x+\int_0^lG(x,\xi)f(\xi)\,d\xi.}
$$

In the final [heat equation](../../../../../heat-equation.md), a [steady state](../../../../../steady-state.md) has zero time [derivative](../../../../../derivative.md). Here $l=1$, $f(x)=x$, $\alpha=1/D$, $\beta=2/D$. Integrating $u''=-x/D$ twice and imposing the endpoint values gives

$$
\boxed{u_{\mathrm{steady}}(x)=\frac1D\left(1+\frac76x-\frac16x^3\right).}
$$

Its second [derivative](../../../../../derivative.md) and both [boundary conditions](../../../../../boundary-condition.md) verify the answer directly.

## ↑ Ancestors (10)

1. [16B](../16b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
