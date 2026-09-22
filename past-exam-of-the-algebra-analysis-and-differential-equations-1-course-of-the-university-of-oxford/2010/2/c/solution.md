<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $n\geq2$, take the matrix whose leading $2\times2$ block is $\left(\begin{smallmatrix}0&1\\-1&0\end{smallmatrix}\right)$ and whose other entries are zero. Its square has leading block $-I_2$, so

$$
\boxed{\varphi(A,A)=\operatorname{tr}(A^2)=-2<0.}
$$

This contradicts the [positive definiteness](../../../../positive-definiteness.md) required of an [inner product](../../../../inner-product-split.md). Even the nonzero matrix unit $E_{12}$ has $\varphi(E_{12},E_{12})=0$.

The printed assertion has an exception: **when $n=1$, $\varphi(a,b)=ab$ is an inner product** on $\mathbb R$. Thus the requested failure requires $n\geq2$, a restriction absent from the printed question.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
