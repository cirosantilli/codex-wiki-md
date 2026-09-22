<h1 id="b/5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $V_h$ be the continuous piecewise linear space including both endpoint [hat functions](../../../../../piecewise-linear-hat-function.md). Robin conditions are natural conditions and do not restrict the endpoint values of this space. The [finite element](../../../../../finite-element.md) problem is $u_h\in V_h$, $a(u_h,v_h)=\ell(v_h)$ for all $v_h\in V_h$. [coercivity](../../../../../coercive-function.md) restricted to $V_h$ gives [existence](../../../../../existence.md) and [uniqueness](../../../../../uniqueness.md).

Expanding $u_h=\sum_{j=0}^NU_j\phi_j$ gives $\mathsf A U=F$, where

$$
\boxed{\mathsf A_{ij}=\int_a^b(\phi_j'\phi_i'+x^2\phi_j\phi_i)\,dx+\delta_{i0}\delta_{j0}+\delta_{iN}\delta_{jN},\quad
F_i=\int_a^bf\phi_i\,dx+A\delta_{i0}+B\delta_{iN}.}
$$

The stiffness contribution has diagonal $2/h$ at interior nodes, $1/h$ at endpoints, and adjacent entries $-1/h$. For completeness, the weighted mass contribution has interior diagonal $2hx_i^2/3+h^3/15$, left endpoint diagonal $ha^2/3+ah^2/6+h^3/30$, right endpoint diagonal $hb^2/3-bh^2/6+h^3/30$, and adjacent entry $hx_i^2/6+h^2x_i/6+h^3/20$. All more distant entries vanish. The Robin contribution adds one to each endpoint diagonal.

Symmetry follows from symmetry of the [bilinear form](../../../../../bilinear-form-split.md). If $V\neq0$, nodal independence makes $v_h=\sum_iV_i\phi_i$ nonzero, and $V^T\mathsf AV=a(v_h,v_h)\geq\gamma\|v_h\|_{H^1}^2>0$. Thus the [matrix](../../../../../matrix.md) is **symmetric positive definite**.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
