<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the real [zero-trace Sobolev space](../../../../../zero-trace-sobolev-space.md) $H_0^1(\Omega)$ with [norm](../../../../../norm.md) $\|\nabla u\|_2$. The [Poincaré inequality](../../../../../poincare-inequality.md) on the bounded smooth [domain](../../../../../domain-mathematical-analysis.md) gives $\|u\|_2\leq C_P\|\nabla u\|_2$, making this an equivalent [Sobolev norm](../../../../../sobolev-norm.md). The [weak formulation](../../../../../weak-formulation.md) is to find $u\in H_0^1(\Omega)$ with $u\geq0$ [almost everywhere](../../../../../almost-everywhere.md) and

$$
\boxed{\int_\Omega\nabla u\cdot\nabla v\,dx
=\int_\Omega(1+\sqrt u)v\,dx\qquad\text{for every }v\in H_0^1(\Omega).}
$$

The zero [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) is encoded in the [Sobolev trace](../../../../../trace-operator.md). Formally, the identity follows by multiplying the [partial differential equation](../../../../../partial-differential-equation-split.md) by a [test function](../../../../../test-function.md) and using [integration by parts](../../../../../integration-by-parts.md); it then extends to all $v\in H_0^1(\Omega)$ by density.

To check all terms, boundedness of $\Omega$ gives finite [Lebesgue measure](../../../../../lebesgue-measure.md) $m=|\Omega|$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $u\in L^1(\Omega)$ and

$$
\|\sqrt u\|_2^2=\int_\Omega u\,dx\leq m^{1/2}\|u\|_2,
\qquad
\|1+\sqrt u\|_2\leq m^{1/2}+m^{1/4}\|u\|_2^{1/2}.
$$

Thus the right side is a bounded [linear functional](../../../../../linear-functional.md) of $v$, since its absolute value is at most $\|1+\sqrt u\|_2 C_P\|\nabla v\|_2$. The left side is finite by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). These estimates work for every stated $n\geq2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../split.md)
6. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
