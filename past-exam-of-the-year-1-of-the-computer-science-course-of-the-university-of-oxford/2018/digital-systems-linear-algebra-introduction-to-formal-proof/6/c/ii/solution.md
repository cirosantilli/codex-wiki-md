<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**No, except when started at the exact solution.** Merely failing the usual [symmetric positive-definite matrix](../../../../../../symmetric-positive-definite-matrix.md) hypothesis would not by itself prove divergence. For this particular matrix one can prove that every defined nonzero-residual step increases the [linear-system residual norm](../../../../../../linear-system-residual-norm.md).

Write $r=(x,y)^T$, put $D=r^TAr=2x^2-2xy-2y^2$ and $B=5x^2+4xy+3y^2$. For $D\ne0$, direct substitution into the stated iteration gives

$$
r^+=r-\frac{r^Tr}{D}Ar=\frac{B}{D}\begin{pmatrix}-y\\x\end{pmatrix},\qquad \|r^+\|=\frac{B}{|D|}\|r\|.
$$

For $r\ne0$, both

$$
B+D=7x^2+2xy+y^2>0,\qquad B-D=3x^2+6xy+5y^2>0
$$

are strictly positive; completing squares gives $7(x+y/7)^2+6y^2/7$ and $3(x+y)^2+2y^2$. Hence $B>|D|$ and the residual norm strictly increases at every defined step. If $D=0$ before the residual vanishes, the algorithm is instead undefined. Neither behavior converges to residual zero. The matrix is invertible, so this also rules out convergence of the iterates to its unique solution.

For example, from the zero starting guess the first two step sizes are $37/11$ and $-37/11$, giving $r_1=(42,30)^T$ and $r_2=(1380/11)r_0$. This demonstrates the failure without treating a sufficient convergence theorem as a necessary one. The general calculation is [residual growth in an indefinite steepest-descent iteration](../../../../../../residual-growth-in-an-indefinite-steepest-descent-iteration.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
