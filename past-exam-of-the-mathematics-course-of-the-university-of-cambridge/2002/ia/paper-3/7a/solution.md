<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

For the [linear map](../../../../../linear-map.md) $\alpha$ represented by $A$, a solution to the [system of linear equations](../../../../../system-of-linear-equations.md) exists precisely when $b\in\operatorname{im}\alpha$. If $x_0$ is one solution, then

$$
Ax=b\iff A(x-x_0)=0\iff x\in x_0+\ker\alpha.
$$

Thus the [affine solution space of a linear equation](../../../../../affine-solution-space-of-a-linear-equation.md) completely describes the possibilities: **no solutions** when $b\notin\operatorname{im}\alpha$; **one solution** when $b\in\operatorname{im}\alpha$ and $\ker\alpha=\{0\}$; and **infinitely many solutions** when $b\in\operatorname{im}\alpha$ and $\ker\alpha\neq\{0\}$. In the last case, a nonzero $w\in\ker\alpha$ supplies the distinct solutions $x_0+tw$ for every real $t$. In dimension three, the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) also says that a trivial [kernel](../../../../../kernel-of-a-linear-map.md) is equivalent to an invertible [matrix](../../../../../matrix.md) $A$.

For the [matrix](../../../../../matrix.md) equation, $AX=B$ means that $\beta=\alpha\circ\chi$, where $\chi$ is represented by $X$. Necessarily $\operatorname{im}\beta\subseteq\operatorname{im}\alpha$. Conversely, if that containment holds, choose an $\alpha$-preimage of each $\beta(e_j)$ for the three standard [basis vectors](../../../../../basis-vector.md), and use those preimages as the columns of $X$. Their linear extension gives $AX=B$. This proves the [image criterion for a matrix factorization](../../../../../image-criterion-for-a-matrix-factorization.md):

$$
\boxed{AX=B\text{ is solvable}\iff\operatorname{im}\beta\subseteq\operatorname{im}\alpha.}
$$

Whenever it is solvable, every solution is $X_0+N$ with $AN=0$. It is unique exactly when $\ker\alpha=\{0\}$. Indeed, a nonzero $w\in\ker\alpha$ produces a nonzero [matrix](../../../../../matrix.md) $N$ with first column $w$ and other columns zero, so uniqueness fails for any compatible $B$ if the [kernel](../../../../../kernel-of-a-linear-map.md) is nontrivial.

For the printed numerical [matrix](../../../../../matrix.md) $A$, its [determinant](../../../../../determinant.md) is $-2$, so the solution is unique. To calculate it, solve $A(x,y,z)^T=(b_1,b_2,b_3)^T$. The last equation gives $z=b_3-3y$; the second then gives $x=b_2-b_3+y$. Substitution into the first yields

$$
y=\frac{b_1-4b_2+3b_3}{2},\quad
x=\frac{b_1-2b_2+b_3}{2},\quad
z=\frac{-3b_1+12b_2-7b_3}{2}.
$$

Applying these formulas to the three columns of the PDF's $B$ gives

$$
\boxed{X=\begin{pmatrix}2&0&3/2\\5&0&7/2\\-12&1&-17/2\end{pmatrix}.}
$$

Multiplication gives $AX=\begin{pmatrix}1&1&1\\0&1&0\\3&1&2\end{pmatrix}$, confirming the result against the printed [matrix](../../../../../matrix.md).

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
