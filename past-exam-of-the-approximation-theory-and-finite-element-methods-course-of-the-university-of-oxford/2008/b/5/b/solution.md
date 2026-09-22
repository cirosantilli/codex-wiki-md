<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $V_h$ be the space spanned by all $N+1$ hats, including the endpoint hats. The solution in a [conforming finite element space](../../../../../conforming-finite-element-space.md) satisfies $a(u_h,v_h)=\ell(v_h)$ for all $v_h\in V_h$. The continuous form remains [coercive](../../../../../coercive-bilinear-form.md) and continuous on this subspace, so the discrete solution is unique.

With $u_h=\sum_jU_j\varphi_j$, its equations are

$$
\boxed{AU=F,\qquad
A_{ij}=\int_0^1(\varphi_i'\varphi_j'+\cos x\,\varphi_i\varphi_j)
+\delta_{i0}\delta_{j0}+\delta_{iN}\delta_{jN},\quad
F_i=\int_0^1f\varphi_i.}
$$

The formula is symmetric in $i,j$. For a nonzero vector $V$, the corresponding spline $v_h=\sum_jV_j\varphi_j$ is nonzero by basis independence, and

$$
V^TAV=a(v_h,v_h)\geq\cos1\,\|v_h\|_{H^1}^2>0.
$$

Thus **$A$ is symmetric positive definite**, proving algebraic solvability as well.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
