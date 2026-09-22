<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $v\ne0$ so that the change of variables is invertible. The [chain rule](../../../../chain-rule.md) gives $\partial_x=\partial_r+\partial_s$ and $\partial_t=v(\partial_r-\partial_s)$. Commuting the [mixed partial derivatives](../../../../mixed-partial-derivative.md) for a twice continuously differentiable solution gives

$$
\partial_x^2-\frac1{v^2}\partial_t^2
=(\partial_r+\partial_s)^2-(\partial_r-\partial_s)^2=4\partial_r\partial_s.
$$

Thus the [wave equation](../../../../wave-equation-split.md) is $F_{rs}=0$. Integrating once says that $F_r$ depends only on $r$; integrating again gives

$$
\boxed{F(x,t)=f(x+vt)+g(x-vt).}
$$

The two arbitrary twice differentiable functions are waves moving in opposite directions at speed $|v|$. This is [D'Alembert's formula](../../../../d-alembert-s-formula.md), on a product domain in $(r,s)$ or globally on the usual full line.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
