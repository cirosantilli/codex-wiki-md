<h1 id="30c/solution">Solution</h1>

↑ **Parent:** [30C](../30c.md)

A [fundamental solution](../../../../../fundamental-solution-of-a-linear-differential-operator.md) of a linear [differential operator](../../../../../differential-operator.md) $P$ is a [distribution](../../../../../distribution-mathematical-analysis.md) $G$ satisfying $PG=\delta_0$. The locally integrable function $G=e^{-|x|}/2$ defines a [distribution](../../../../../distribution-mathematical-analysis.md) by integration against compactly supported smooth test [functions](../../../../../function-split.md). Away from zero it satisfies $-G''+G=0$. It is continuous at zero, while $G'(0+)=-1/2$ and $G'(0-)=1/2$. Consequently its distributional second derivative is its ordinary derivative on the two sides plus the derivative jump times $\delta_0$:

$$
G''=G-\delta_0,\qquad\boxed{(-d^2/dx^2+1)G=\delta_0.}
$$

This derivative-jump formula follows by [integration by parts](../../../../../integration-by-parts.md) on each half-line; the boundary terms equal $-\phi(0)$ in $G''$.

[Convolution](../../../../../convolution.md) with the indicator forcing gives

$$
u_0(x)=\frac12\int_{-1}^1e^{-|x-y|}\,dy
=\boxed{\begin{cases}1-e^{-1}\cosh x,&|x|\leq1,\\
\sinh(1)e^{-|x|},&|x|\geq1.\end{cases}}
$$

The two values and their first derivatives agree at $\pm1$, so no delta terms arise there. This is a decaying [weak solution](../../../../../weak-solution.md), with the equation holding classically away from the forcing jumps.

For real Schwartz $\phi$, expand the [energy](../../../../../energy.md):

$$
I[u_0+\phi]-I[u_0]
=\int(u_0'\phi'+u_0\phi-V\phi)\,dx
+\frac12\int[(\phi')^2+\phi^2]\,dx.
$$

The mixed term is zero by the weak equation $-u_0''+u_0=V$, or [integration by parts](../../../../../integration-by-parts.md) using the continuous first derivative and decay. The remaining integral is strictly positive whenever $\phi$ is not identically zero. Hence

$$
\boxed{I[u_0+\phi]>I[u_0]\quad(0\ne\phi\text{ a real Schwartz function}).}
$$

The real-valued function space is implicit in the stated ordered quadratic functional; for complex [functions](../../../../../function-split.md) one instead uses absolute squares and the corresponding real part of the forcing term.

## ↑ Ancestors (10)

1. [30C](../30c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
