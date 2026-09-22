<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

Write the [linear system of differential equations](../../../../../linear-system-of-differential-equations.md) as

$$
\mathbf z'=\frac1tA\mathbf z+\mathbf b,\qquad
A=\begin{pmatrix}4&-2\\-1&5\end{pmatrix},\quad\mathbf b=\binom{-9}{3}.
$$

A homogeneous power $t^\lambda\mathbf v$ solves this [Cauchy-Euler differential system](../../../../../cauchy-euler-differential-system.md) precisely when $A\mathbf v=\lambda\mathbf v$. The [eigenvalues](../../../../../eigenvalue.md) are $3$ and $6$, with [eigenvectors](../../../../../eigenvector.md) $(2,1)^T$ and $(1,-1)^T$. The homogeneous solution is therefore $C t^3(2,1)^T+D t^6(1,-1)^T$.

For a particular solution, put $\mathbf z_p=t\mathbf c$. Then $(I-A)\mathbf c=\mathbf b$, which gives $\mathbf c=(3,0)^T$. At $t=1$, the two initial conditions become $2C+D+3=0$ and $C-D=0$, so $C=D=-1$. Thus

$$
\boxed{x(t)=3t-2t^3-t^6,\qquad y(t)=t^6-t^3,\qquad t\geq1}.
$$

The two powers correspond to the two [eigenvalues](../../../../../eigenvalue.md); the lower-degree particular term accounts for the constant forcing. Substitution gives both original right sides and the zero initial data.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
