<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\lambda\ne0$, factor the matrix inside the [determinant](../../../../../determinant.md):

$$
\begin{aligned}
\chi_M(\lambda)
&=\det M\,\det(\lambda M^{-1}-I)\\
&=\lambda^{2m}\det(M^{-1}-\lambda^{-1}I)\\
&=\lambda^{2m}\det(\lambda^{-1}I-M^{-1})\\
&=\lambda^{2m}\chi_M(\lambda^{-1}).
\end{aligned}
$$

The second line uses $\det M=1$; the third uses the even matrix size; the last uses part (i). Consequently

$$
\boxed{\chi_M(\lambda)=\lambda^{2m}\chi_M(\lambda^{-1}).}
$$

In other words, the [characteristic polynomial](../../../../../characteristic-polynomial.md) equals its [reciprocal polynomial](../../../../../reciprocal-polynomial.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
