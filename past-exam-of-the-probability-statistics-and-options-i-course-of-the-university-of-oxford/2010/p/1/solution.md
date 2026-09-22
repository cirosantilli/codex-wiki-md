<h1 id="p/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Eliminate the first column with multipliers $\ell_{21}=2$ and $\ell_{31}=-1$. The new second and third rows are $(0,2,4)$ and $(0,-1,3)$. The next multiplier is $\ell_{32}=-1/2$, giving final row $(0,0,5)$. Recording these multipliers gives the [LU decomposition](../../../../lu-decomposition.md)

$$
\boxed{L=\begin{pmatrix}1&0&0\\2&1&0\\-1&-1/2&1\end{pmatrix},\qquad
U=\begin{pmatrix}1&2&2\\0&2&4\\0&0&5\end{pmatrix},\qquad A=LU.}
$$

For an upper-triangular [matrix](../../../../matrix.md) with nonzero diagonal, the [back substitution](../../../../back-substitution.md) algorithm works from bottom to top:

$$
x_i=\frac{b_i-\sum_{j=i+1}^n u_{ij}x_j}{u_{ii}},\qquad i=n,n-1,\ldots,1.
$$

In the separate triangular system printed in the question, $5x_3=10$, $2x_2+4x_3=6$, and $x_1+2x_2+2x_3=3$. Hence

$$
\boxed{x=(1,-1,2)^{\mathsf T}.}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [P](../../p.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
