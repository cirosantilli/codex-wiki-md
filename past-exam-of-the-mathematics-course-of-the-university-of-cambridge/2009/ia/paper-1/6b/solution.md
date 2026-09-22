<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

For any [linear system](../../../../../system-of-linear-equations.md) $Ax=c$, a solution exists exactly when $c$ belongs to the [image of a linear map](../../../../../image-of-a-linear-map.md) represented by $A$. If $x_0$ is one solution, all others are exactly

$$
x=x_0+v,\qquad v\in\ker A,
$$

since $A(x-x_0)=0$, and conversely adding a [kernel](../../../../../kernel-of-a-linear-map.md) [vector](../../../../../vector.md) preserves the equation. Thus there are no solutions if $c\notin\operatorname{im}A$, one if $c\in\operatorname{im}A$ and $\ker A=\{0\}$, and infinitely many if $c\in\operatorname{im}A$ and the [kernel](../../../../../kernel-of-a-linear-map.md) is nontrivial: every real multiple of a nonzero [kernel](../../../../../kernel-of-a-linear-map.md) [vector](../../../../../vector.md) gives a distinct solution. Any two solutions differ by a [kernel](../../../../../kernel-of-a-linear-map.md) [vector](../../../../../vector.md). Equivalently, consistency means the augmented [matrix](../../../../../matrix.md) and $A$ have equal [rank of a matrix](../../../../../matrix-rank.md); a consistent square [linear system](../../../../../system-of-linear-equations.md) is unique exactly when its [determinant](../../../../../determinant.md) is nonzero.

For the given [matrix](../../../../../matrix.md), set $d=b-a$ and $s=2a+b$. Perform the [column operation](../../../../../elementary-column-operation.md) $C_1\leftarrow C_1+C_2+C_3$, then the [row operations](../../../../../elementary-row-operation.md) $R_2\leftarrow R_2-R_1$ and $R_3\leftarrow R_3-R_1$. Factoring the first column gives

$$
\det A=s\det\begin{pmatrix}1&a&b\\0&0&a-b\\0&b-a&a-b\end{pmatrix}
=\boxed{(2a+b)(b-a)^2}.
$$

These operations are determinant-preserving, and the displayed polynomial identity remains valid even when a factored expression vanishes.

To find all [kernels](../../../../../kernel-of-a-linear-map.md) and [images of a linear map](../../../../../image-of-a-linear-map.md), put

$$
u=(1,1,1)^T,\qquad H=\{x:x_1+x_2+x_3=0\},\qquad P=\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix}.
$$

If $J$ is the all-ones [matrix](../../../../../matrix.md), then $A=aJ+dP$. The [direct sum](../../../../../direct-sum.md) $\mathbb R^3=\mathbb Ru\oplus H$ is invariant under $A$: on $\mathbb Ru$ it acts by multiplication by $s$, and on $H$ by $dP$. Since $P^3=I$, its restriction to $H$ is invertible.

For $d\ne0$ and $s\ne0$, the [kernel](../../../../../kernel-of-a-linear-map.md) is $\{0\}$ and the [image of a linear map](../../../../../image-of-a-linear-map.md) is all of $\mathbb R^3$. Decompose the right-hand side as

$$
(1,c,1)^T=\frac{c+2}{3}u+\frac{c-1}{3}(-1,2,-1)^T.
$$

Applying the inverse on each invariant summand gives the unique solution

$$
\boxed{x=\frac{c+2}{3s}u+\frac{c-1}{3d}(2,-1,-1)^T.}
$$

For $d\ne0$ and $s=0$, the [kernel](../../../../../kernel-of-a-linear-map.md) is $\mathbb Ru$ and the [image of a linear map](../../../../../image-of-a-linear-map.md) is $H$. A solution exists exactly when $c+2=0$. For $c=-2$, all solutions are

$$
\boxed{x=-\frac1d(2,-1,-1)^T+t u,\qquad t\in\mathbb R.}
$$

For $d=0$ and $a\ne0$, so $a=b$, the [kernel](../../../../../kernel-of-a-linear-map.md) is $H$ and the [image of a linear map](../../../../../image-of-a-linear-map.md) is $\mathbb Ru$. A solution exists exactly when $c=1$. All such solutions are

$$
\boxed{x=(r,t,1/a-r-t)^T,\qquad r,t\in\mathbb R.}
$$

Finally, for $a=b=0$, the [kernel](../../../../../kernel-of-a-linear-map.md) is $\mathbb R^3$ and the [image of a linear map](../../../../../image-of-a-linear-map.md) is $\{0\}$. The right-hand side has first entry one, so **there is no solution for any $c$**. These four cases exhaust all parameter values.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
