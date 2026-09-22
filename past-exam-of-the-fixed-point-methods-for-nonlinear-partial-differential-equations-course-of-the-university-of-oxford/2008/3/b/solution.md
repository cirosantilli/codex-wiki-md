<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the [zero-boundary Sobolev space](../../../../zero-boundary-sobolev-space.md) $X=H_0^1(\Omega)$ with norm $\|u\|_X=\|\nabla u\|_2$. The [Poincaré inequality](../../../../poincare-inequality.md) makes this equivalent to the usual [Sobolev norm](../../../../sobolev-norm.md). Define

$$
\boxed{\langle A(u),v\rangle=\int_\Omega\nabla u\cdot\nabla v+\int_\Omega u^3v,\qquad\langle f,v\rangle=\int_\Omega v.}
$$

The [weak formulation](../../../../weak-formulation.md) is $u\in X$ and $\langle A(u),v\rangle=\langle f,v\rangle$ for every $v\in X$.

In dimension three the [Sobolev embedding theorem](../../../../sobolev-embedding-theorem.md) gives $\|u\|_6\leq C_6\|u\|_X$, so $u^3\in L^2$. The [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) and [Poincaré inequality](../../../../poincare-inequality.md) yield

$$
|\langle A(u),v\rangle|\leq\bigl(\|u\|_X+C_PC_6^3\|u\|_X^3\bigr)\|v\|_X,
\qquad|\langle f,v\rangle|\leq|\Omega|^{1/2}C_P\|v\|_X.
$$

Thus $A(u)\in X^*$ for every $u$, and $f\in X^*$. Finally

$$
\begin{aligned}
\langle A(u)-A(w),u-w\rangle
&=\|u-w\|_X^2+\int_\Omega(u-w)^2(u^2+uw+w^2)\\
&\geq\boxed{\|u-w\|_X^2},
\end{aligned}
$$

since $u^2+uw+w^2\geq0$. Hence $A$ is strongly monotone with constant one in the chosen norm.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
