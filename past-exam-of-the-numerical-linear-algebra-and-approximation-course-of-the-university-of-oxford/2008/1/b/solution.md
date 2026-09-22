<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $x\ne0$, choose $\alpha=-\operatorname{sgn}(x_1)\|x\|_2$, with $\operatorname{sgn}(0)=1$ for this choice, and put $v=x-\alpha e_1$. This nonzero vector satisfies

$$
v^Tx=\|x\|_2^2-\alpha x_1,\qquad v^Tv=2(\|x\|_2^2-\alpha x_1).
$$

Thus the [Householder matrix](../../../../householder-transformation.md) $H=I-2vv^T/(v^Tv)$ gives $Hx=x-v=\alpha e_1$. Symmetry gives $\boxed{x^TH=\alpha e_1^T}$. If $x=0$, any [Householder matrix](../../../../householder-transformation.md) works with $\alpha=0$.

For an [LQ decomposition](../../../../lq-decomposition.md), process rows $j=1,\ldots,\min(m,n)$. At step $j$, postmultiply by an orthogonal block matrix $H_j=\operatorname{diag}(I_{j-1},\widehat H_j)$ that zeros entries to the right of the diagonal in the current row. If its row tail is already suitable, use the identity. Earlier processed rows have zero entries throughout this trailing block, so their zeros are preserved. Consequently $L=AH_1\cdots H_r$ has $l_{ij}=0$ for $i<j$. Setting $\boxed{Q=H_r^T\cdots H_1^T}$ gives $\boxed{A=LQ}$. The argument handles both rectangular shapes; $L$ is lower trapezoidal when it is not square.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the numerical linear algebra and approximation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and approximation course of the University of Oxford](../../../../numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
