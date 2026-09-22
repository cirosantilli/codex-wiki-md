<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the unweighted [inner product](../../../../../inner-product-split.md) $\langle w,y\rangle=\int_0^a\overline w y\,dx$. Two applications of [integration by parts](../../../../../integration-by-parts.md) give

$$
\int_0^a\overline w(y''+2y'+2y)\,dx
=\int_0^a(\overline w''-2\overline w'+2\overline w)y\,dx
+[\overline w y'-\overline w'y+2\overline w y]_0^a.
$$

The given [boundary conditions](../../../../../boundary-condition.md) set $y=0$ at both ends, but leave $y'(0)$ and $y'(a)$ independently variable. The remaining boundary term vanishes for every admissible $y$ precisely when $w(0)=w(a)=0$. Consequently the [formal adjoint](../../../../../formal-adjoint.md) and the boundary conditions specifying the [adjoint operator](../../../../../adjoint-operator.md) are

$$
\boxed{\mathcal L^*w=w''-2w'+2w,\qquad w(0)=w(a)=0}.
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
