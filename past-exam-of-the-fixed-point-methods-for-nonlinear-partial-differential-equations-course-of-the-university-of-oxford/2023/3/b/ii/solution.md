<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the spaces in part (b)(i) and fixed $f\in Y$, define $A:X\to X^*$ by

$$
\boxed{\langle A(u),v\rangle
=\int_\Omega|\nabla u|^2\nabla u\cdot\nabla v\,dx
+\int_\Omega u^7v\,dx-\int_\Omega fv\,dx.}
$$

For each $u$, this is a [linear functional](../../../../../linear-functional.md) in $v$, and the estimates in part (b)(i) show

$$
\|A(u)\|_{X^*}\leq\|u\|_X^3+C_8^8\|u\|_X^7+C_8\|f\|_{8/7}.
$$

Hence $A(u)$ belongs to the [continuous dual space](../../../../../continuous-dual-space-split.md) $X^*$, and $A$ sends bounded [sets](../../../../../set-split.md) to bounded [sets](../../../../../set-split.md). The [weak formulation](../../../../../weak-formulation.md) is exactly

$$
\boxed{\langle A(u),v\rangle=0\quad\forall v\in X,\quad\text{equivalently }A(u)=0\text{ in }X^*.}
$$

The forcing term is included in $A$ so that its right side is zero, as requested.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
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
