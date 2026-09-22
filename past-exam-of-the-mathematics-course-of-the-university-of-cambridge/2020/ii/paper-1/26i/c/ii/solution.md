<h1 id="26i/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Consider the smooth map

$$
\Psi:M_4(\mathbb R)\to\operatorname{Sym}_4(\mathbb R),
\qquad
\Psi(A)=A^TMA.
$$

Its derivative is

$$
D\Psi_A(H)=H^TMA+A^TMH.
$$

At $A\in O(1,3)$ write $H=AY$. Then

$$
D\Psi_A(AY)=Y^TM+MY.
$$

This derivative is onto the ten-dimensional space of symmetric matrices: for a symmetric $S$, taking $Y=\tfrac12MS$ gives $Y^TM+MY=S$. Hence $M$ is a regular value. Since $M_4(\mathbb R)$ has dimension 16, the [regular level set theorem](../../../../../../../regular-level-set-theorem.md) gives

$$
\boxed{\dim O(1,3)=16-10=6}.
$$

The tangent vectors are exactly those for which the derivative vanishes:

$$
\boxed{
T_AO(1,3)=\{AY:Y\in\mathfrak S\},
\qquad
\mathfrak S=\{Y:Y^TM+MY=0\}.
}
$$

Writing $Y$ in one-plus-three block form shows explicitly that

$$
\mathfrak S
=\left\{
\begin{pmatrix}
0&v^T\\
v&\Omega
\end{pmatrix}
:v\in\mathbb R^3,\ \Omega^T=-\Omega
\right\}.
$$

The three entries of $v$ and three independent entries of the skew-symmetric matrix $\Omega$ again display dimension six. This is the [Lie algebra of the Lorentz group](../../../../../../../lie-algebra-of-the-lorentz-group.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [26I](../../../26i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
