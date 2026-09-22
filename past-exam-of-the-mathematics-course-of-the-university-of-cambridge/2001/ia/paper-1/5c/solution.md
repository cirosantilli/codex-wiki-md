<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

To find the [kernel of a linear map](../../../../../kernel-of-a-linear-map.md), perform the row operations $R_2\leftarrow R_2-R_1$ and $R_3\leftarrow R_3-(1+\alpha)R_1$, followed by $R_3\leftarrow R_3-R_2$. The equivalent homogeneous equations are

$$
x-y+(2\alpha+1)z=0,\qquad \alpha y-2\alpha z=0,\qquad \alpha(3-\alpha)z=0.
$$

The resulting [determinant](../../../../../determinant.md) is $\alpha^2(3-\alpha)$. If $\alpha\notin\{0,3\}$ all coordinates vanish. At $\alpha=0$ only $x-y+z=0$ remains; at $\alpha=3$ the equations give $y=2z$, $x=-5z$. Therefore **kernel bases are**

$$
\boxed{\begin{cases}
\varnothing,&\alpha\notin\{0,3\},\\
\{(1,1,0)^T,(-1,0,1)^T\},&\alpha=0,\\
\{(-5,2,1)^T\},&\alpha=3.
\end{cases}}
$$

The empty family is the [basis](../../../../../basis.md) of the zero [vector subspace](../../../../../vector-subspace.md).

For the [change of basis](../../../../../change-of-basis.md), let $B_0,C_0$ be the matrices whose columns are the two ordered bases in standard coordinates. Then $v=B_0[v]_B=C_0[v]_C$, so $[v]_B=S[v]_C$ with $S=B_0^{-1}C_0$. If $A$ and $A'$ represent the same [linear map](../../../../../linear-map.md) in the two bases, $[\Phi(v)]_B=A[v]_B$ and also $[\Phi(v)]_B=SA'[v]_C$. Therefore $SA'=AS$, and

$$
\boxed{A'=S^{-1}AS,\qquad S=B_0^{-1}C_0.}
$$

For the concrete bases, their vectors satisfy $c_1=b_1+b_2$, $c_2=b_2+b_3$, $c_3=b_1+b_2+b_3$. These coordinate columns give

$$
\boxed{S=\begin{pmatrix}1&0&1\\1&1&1\\0&1&1\end{pmatrix},\qquad
S^{-1}=\begin{pmatrix}0&1&-1\\-1&1&0\\1&-1&1\end{pmatrix}.}
$$

At $\alpha=0$, every row of $A_0$ is $(1,-1,1)$, so every row of $A_0S$ is $(0,0,1)$. Multiplying on the left by the displayed inverse gives

$$
\boxed{S^{-1}A_0S=\begin{pmatrix}0&0&0\\0&0&0\\0&0&1\end{pmatrix}.}
$$

The original PDF asks for this full product; its final factor $S$ is missing from the converted TeX.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
