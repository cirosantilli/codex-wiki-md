<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [gradient](../../../../../../../gradient.md) and constant [Hessian matrix](../../../../../../../hessian-matrix.md) are

$$
\nabla F=\begin{pmatrix}6x-4y+4\\4y-4x-4\end{pmatrix},\qquad
H_F=\begin{pmatrix}6&-4\\-4&4\end{pmatrix},\qquad
H_F^{-1}=\frac18\begin{pmatrix}4&4\\4&6\end{pmatrix}.
$$

At $\mathbf x_0=(1,0)^T$, $\nabla F=(10,-8)^T$ and $H_F^{-1}\nabla F=(1,-1)^T$. Hence one [multivariable Newton iteration](../../../../../../../multivariable-newton-iteration.md) gives

$$
\boxed{\mathbf x_1=(1,0)^T-(1,-1)^T=(0,1)^T.}
$$

At this point the [gradient](../../../../../../../gradient.md) vanishes, so every subsequent iterate is $(0,1)$. The one-step result follows because the [gradient](../../../../../../../gradient.md) of a quadratic [polynomial](../../../../../../../polynomial-split.md) is affine and its linearization is exact. Since the leading principal minors of $H_F$ are $6>0$ and $8>0$, it is a [positive-definite matrix](../../../../../../../positive-definite-matrix.md). Alternatively,

$$
F(x,y)=x^2+2(y-x-1)^2-1
$$

directly proves that **$(0,1)$ is the unique [global minimum](../../../../../../../global-minimum.md), with value $-1$**.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
