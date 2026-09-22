<h1 id="14a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $s=\log x$ and $Y(s)=y(e^s)$, so $0\leq s\leq1$. By the [chain rule](../../../../../../../chain-rule.md), the equation becomes $Y''+2Y'+(1+\lambda)Y=0$. The substitution $Y=e^{-s}v$ reduces it further to

$$
v''+\lambda v=0,\qquad v(0)=v(1)=0.
$$

Multiplication by $\overline v$ and [integration by parts](../../../../../../../integration-by-parts.md) gives $\lambda\int_0^1|v|^2=\int_0^1|v'|^2>0$ for a nonzero solution, ruling out zero and negative [eigenvalues](../../../../../../../eigenvalue.md). For $\lambda=k^2>0$, the first boundary condition gives $v=A\sin(ks)$, and the second gives $k=n\pi$, $n=1,2,\ldots$. Thus **all eigenpairs are**

$$
\boxed{\lambda_n=n^2\pi^2,\qquad y_n(x)=\frac1x\sin(n\pi\log x),\quad n\geq1,}
$$

with arbitrary nonzero scalar multiples of each [eigenfunction](../../../../../../../eigenfunction.md). These are the complete list since all solutions of the constant-coefficient [differential equation](../../../../../../../differential-equation-split.md) have been considered; the transformed sine system is also complete in the corresponding weighted [Hilbert space](../../../../../../../hilbert-space-split.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [14A](../../../14a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ib](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
