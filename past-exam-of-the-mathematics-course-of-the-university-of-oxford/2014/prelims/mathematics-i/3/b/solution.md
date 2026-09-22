<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Solve $Ax=b$ for a general right-hand side $b=(b_1,b_2,b_3,b_4)^T$. Subtracting the fourth equation from the second gives $x_3=b_2-b_4$. The first and fourth then give

$$
x_1=b_1-b_2+b_4-x_4,\qquad x_2=b_4-x_4.
$$

Substitution into the third equation reduces the remaining condition to

$$
(t-2)x_4=b_3-b_1-b_4.
$$

If $t\ne2$, every right-hand side therefore has a unique solution, and collecting its four coefficients yields the [matrix inverse](../../../../../../matrix-inverse-split.md)

$$
\boxed{A^{-1}=\frac1{t-2}
\begin{pmatrix}
t-1&2-t&-1&t-1\\
1&0&-1&t-1\\
0&t-2&0&2-t\\
-1&0&1&-1
\end{pmatrix},\qquad t\ne2.}
$$

For $t=2$, the nonzero [vector](../../../../../../vector.md) $(-1,-1,0,1)^T$ lies in the [kernel of a linear map](../../../../../../kernel-of-a-linear-map-split.md) represented by $A$, so $A$ is singular. Hence **$A$ is invertible exactly when $t\ne2$**. The same calculation gives $\det A=t-2$; the formula above can also be checked by multiplying its numerator by $A$ to obtain $(t-2)I$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
