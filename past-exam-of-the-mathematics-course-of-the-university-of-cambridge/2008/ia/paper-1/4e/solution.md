<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

Fix $x\in(0,1)$. For any sufficiently small nonzero $h$, the additivity of the [Riemann integral](../../../../../riemann-integral.md) gives

$$
\frac{F(x+h)-F(x)}h-f(x)
=\frac1h\int_x^{x+h}[f(t)-f(x)]\,dt.
$$

Taking absolute values, for either sign of $h$,

$$
\left|\frac{F(x+h)-F(x)}h-f(x)\right|
\leq\sup_{|t-x|\leq|h|}|f(t)-f(x)|.
$$

Because $f$ is [continuous](../../../../../continuous-function.md) at $x$, the right side tends to zero. Thus the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) here follows directly from the difference quotient:

$$
\boxed{F'(x)=f(x)\quad(0<x<1).}
$$

Only [continuity](../../../../../continuous-function.md) at the point under consideration was used.

Without [continuity](../../../../../continuous-function.md), the assertion is false. Take the [Riemann integrable](../../../../../riemann-integrable-function.md) step function $f(t)=0$ for $t<1/2$ and $f(t)=1$ for $t\geq1/2$. Its primitive is $F(x)=0$ for $x\leq1/2$ and $F(x)=x-1/2$ for $x\geq1/2$. The left and right difference quotients at $1/2$ are respectively zero and one, so **the primitive need not be differentiable at every interior point**. A function with this single jump is [Riemann integrable](../../../../../riemann-integrable-function.md); changing its value at the jump does not change the [integral](../../../../../integral.md) or the counterexample.

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
