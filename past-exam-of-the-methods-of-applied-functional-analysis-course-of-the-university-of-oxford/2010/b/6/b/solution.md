<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [graph area functional](../../../../../graph-area-functional.md) is finite on $H^1$, since $\sqrt{1+|\nabla u|^2}\leq1+|\nabla u|$ and $\Omega$ has finite volume. For $p=\nabla u$, $q=\nabla v$, the difference quotient of $\sqrt{1+|p+tq|^2}$ is bounded in absolute value by $|q|$. This is integrable by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore gives

$$
\boxed{\partial_vF(u)=\langle A(u),v\rangle=\int_\Omega\frac{\nabla u\cdot\nabla v}{\sqrt{1+|\nabla u|^2}}\,dx.}
$$

This defines a bounded [linear functional](../../../../../linear-functional.md) of $v$, since $|\langle A(u),v\rangle|\leq|\Omega|^{1/2}\|\nabla v\|_2$.

For $a(p)=p/\sqrt{1+|p|^2}$ the [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
Da(p)=\frac{I}{\sqrt{1+|p|^2}}-\frac{pp^T}{(1+|p|^2)^{3/2}},\qquad
q^TDa(p)q=\frac{(1+|p|^2)|q|^2-(p\cdot q)^2}{(1+|p|^2)^{3/2}}\geq0.
$$

The inequality follows from the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Integrating this derivative along the segment between any two gradients shows $(a(p)-a(r))\cdot(p-r)\geq0$. Integrating over $\Omega$ proves that $A$ is a [monotone operator](../../../../../monotone-operator.md).

It is **not coercive on $H^1(\Omega)$**. The constant functions $u_k\equiv k$ satisfy $\|u_k\|_{H^1}=k|\Omega|^{1/2}\to\infty$ but $A(u_k)=0$. Thus $\langle A(u_k),u_k\rangle/\|u_k\|_{H^1}=0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
