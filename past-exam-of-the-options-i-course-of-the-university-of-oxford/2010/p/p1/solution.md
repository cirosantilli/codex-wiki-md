<h1 id="p/p1/solution">Solution</h1>

↑ **Parent:** [P1](../p1.md)

The first elimination multipliers are $l_{21}=2$ and $l_{31}=-1$. Subtracting those multiples of row one gives lower rows $(0,2,4)$ and $(0,-1,3)$. The next multiplier is $l_{32}=-1/2$, and the final elimination produces $(0,0,5)$. Thus

$$
\boxed{L=\begin{pmatrix}1&0&0\\2&1&0\\-1&-1/2&1\end{pmatrix},
\qquad U=\begin{pmatrix}1&2&2\\0&2&4\\0&0&5\end{pmatrix},\qquad A=LU.}
$$

For an upper triangular system $Ux=b$ with nonzero diagonal, [back substitution](../../../../back-substitution.md) computes

$$
\boxed{x_i=\frac{b_i-\sum_{j=i+1}^nu_{ij}x_j}{u_{ii}},
\qquad i=n,n-1,\ldots,1.}
$$

For the supplied triangular system, the last row gives $x_3=10/5=2$; the second gives $x_2=(6-4\cdot2)/2=-1$; the first gives $x_1=3-2(-1)-2(2)=1$. Hence

$$
\boxed{x=(1,-1,2)^T.}
$$

## ↑ Ancestors (12)

1. [P1](../p1.md)
2. [P](../../p.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
