<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the convention that the [inner product](../../../../inner-product-split.md) is linear in its first argument. By the defining identity for the [adjoint operator](../../../../adjoint-operator.md),

$$
\begin{aligned}
x\in(\operatorname{Im}T^*)^\perp
&\Longleftrightarrow\langle x,T^*y\rangle=0\quad\text{for every }y\in X\\
&\Longleftrightarrow\langle Tx,y\rangle=0\quad\text{for every }y\in X\\
&\Longleftrightarrow Tx=0.
\end{aligned}
$$

For the last implication choose $y=Tx$. This proves the first [image-kernel orthogonality for an adjoint](../../../../image-kernel-orthogonality-for-an-adjoint.md) identity. Taking [orthogonal complements](../../../../orthogonal-complement.md) and using the [double orthogonal complement](../../../../double-orthogonal-complement.md) theorem for the [vector subspace](../../../../vector-subspace.md) $\operatorname{Im}T^*$ gives

$$
\boxed{\ker T=(\operatorname{Im}T^*)^\perp,\qquad(\ker T)^\perp=\overline{\operatorname{Im}T^*}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the functional analysis II course of the University of Oxford](../../../split.md)
5. [Functional analysis II course of the University of Oxford](../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
