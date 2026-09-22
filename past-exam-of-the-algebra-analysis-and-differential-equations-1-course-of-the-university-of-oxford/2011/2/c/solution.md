<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [inner product](../../../../inner-product-split.md) with $a=2$. The required first vector $v_1=(1/2,0)^T$ already has squared [norm](../../../../norm.md) $4(1/2)^2=1$. Apply the [Gram-Schmidt process](../../../../gram-schmidt-process.md) to $v_1$ followed by $e_2=(0,1)^T$. Since $\beta(e_2,v_1)=-1$, its orthogonal remainder is $w=e_2+v_1=(1/2,1)^T$. Its squared [norm](../../../../norm.md) is $\beta(w,w)=1-2+3=2$. Therefore an [orthonormal basis](../../../../orthonormal-basis.md) containing the specified vector is

$$
\boxed{\left\{\begin{pmatrix}1/2\\0\end{pmatrix},\quad
\frac1{\sqrt2}\begin{pmatrix}1/2\\1\end{pmatrix}\right\}.}
$$

The second vector may also be replaced by its negative.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
