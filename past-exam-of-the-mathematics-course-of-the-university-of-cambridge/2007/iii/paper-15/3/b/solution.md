<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [curvature form of a connection](../../../../../../curvature-form.md) by the operator

$$
F(X,Y)s=\nabla_X\nabla_Ys-\nabla_Y\nabla_Xs-\nabla_{[X,Y]}s.
$$

It is alternating in $X,Y$. It is also tensorial. For instance, replacing $s$ by $fs$ makes the coefficient of $s$ from derivatives of $f$ equal to $X(Yf)-Y(Xf)-[X,Y]f=0$; the remaining mixed terms $(Xf)\nabla_Ys$ and $(Yf)\nabla_Xs$ cancel between the two second derivatives. Thus $F(X,Y)(fs)=fF(X,Y)s$. Replacing $X$ by $fX$, the unwanted term $-(Yf)\nabla_Xs$ cancels the opposite term from $[fX,Y]=f[X,Y]-(Yf)X$. Hence $F(fX,Y)=fF(X,Y)$, and the other input follows by alternation.

Consequently $F_p$ depends only on the tangent vectors $X_p,Y_p$ and on $s_p$, giving a smooth global element of $\Omega^2(M;\operatorname{End}E)$. In the coefficient-column convention of part (a), applying $d_A$ twice to an arbitrary $E$-valued $r$-form gives

$$
\begin{aligned}
d_A^2\sigma
&=d(d\sigma+A\wedge\sigma)+A\wedge(d\sigma+A\wedge\sigma)\\
&=dA\wedge\sigma-A\wedge d\sigma+A\wedge d\sigma+A\wedge A\wedge\sigma\\
&=(dA+A\wedge A)\wedge\sigma.
\end{aligned}
$$

For sections this agrees with the operator definition, so the local [Cartan curvature matrix equation](../../../../../../cartan-curvature-matrix-equation.md) is

$$
\boxed{F=dA+A\wedge A,\qquad
F_{ij}=\partial_iA_j-\partial_jA_i+[A_i,A_j].}
$$

Here $F=\tfrac12\sum_{i,j}F_{ij}dx^i\wedge dx^j$, with $F_{ij}=F(\partial_i,\partial_j)$. The same calculation for all degrees proves

$$
\boxed{d_A^2\sigma=F\wedge\sigma.}
$$

Under $e'=eg$, applying the covariance of $d_A$ twice gives $F'=g^{-1}Fg$. This is exactly the transition rule of the [endomorphism bundle](../../../../../../endomorphism-bundle.md), independently confirming that $F$ is a well-defined bundle-valued two-form.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
