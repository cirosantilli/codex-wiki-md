<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [comultiplication](../../../../../../comultiplication.md) $\Delta E=E\otimes K+1\otimes E$, $\Delta F=F\otimes1+K^{-1}\otimes F$, $\Delta K=K\otimes K$ of the [quantum enveloping algebra of sl2](../../../../../../quantum-enveloping-algebra-of-sl2.md). Choose a [basis](../../../../../../basis.md) $u_0,u_1$ for $V_{1,1}$ with $Fu_0=u_1$, $Eu_1=u_0$, and $Ku_i=q^{1-2i}u_i$. Choose a [basis](../../../../../../basis.md) $w_0,w_1,w_2$ for $V_{1,2}$ with

$$
Fw_0=w_1,\quad Fw_1=[2]w_2,\quad
Ew_1=[2]w_0,\quad Ew_2=w_1,\quad Kw_j=q^{2-2j}w_j,
$$

and all terminal raising or lowering actions zero. This is one of the corrected [bases](../../../../../../basis.md) from part (a).

In the [tensor product of modules](../../../../../../tensor-product-of-modules.md), put

$$
\begin{aligned}
z_0&=u_0\otimes w_0,\\
z_1&=u_1\otimes w_0+q^{-1}u_0\otimes w_1,\\
z_2&=u_1\otimes w_1+q^{-2}u_0\otimes w_2,\\
z_3&=u_1\otimes w_2.
\end{aligned}
$$

The vector $z_0$ is killed by $E$ and has $K$ [eigenvalue](../../../../../../eigenvalue.md) $q^3$. Direct application of the [comultiplication](../../../../../../comultiplication.md) gives

$$
Fz_0=z_1,\quad Fz_1=[2]z_2,\quad Fz_2=[3]z_3,\quad Fz_3=0,
$$

and the string formula gives $Ez_1=[3]z_0$, $Ez_2=[2]z_1$, $Ez_3=z_2$. Also $Kz_i=q^{3-2i}z_i$. Thus $W_3=\langle z_0,z_1,z_2,z_3\rangle$ is a [submodule](../../../../../../submodule.md) isomorphic to $V_{1,3}$.

The other highest vector and its lowered partner are

$$
\begin{aligned}
h_0&=[2]u_1\otimes w_0-q^2u_0\otimes w_1,\\
h_1=Fh_0&=u_1\otimes w_1-q[2]u_0\otimes w_2.
\end{aligned}
$$

Indeed $Eh_0=([2]q^2-q^2[2])u_0\otimes w_0=0$, $Kh_0=qh_0$, $Kh_1=q^{-1}h_1$, $Eh_1=h_0$ and $Fh_1=0$. Therefore $W_1=\langle h_0,h_1\rangle$ is a [submodule](../../../../../../submodule.md) isomorphic to $V_{1,1}$.

To verify that this is a direct sum, in the $q$ [weight space](../../../../../../weight-space.md) the determinant of the coefficients of $z_1,h_0$ is $-q^2-q^{-1}[2]=-[3]\ne0$. In the $q^{-1}$ [weight space](../../../../../../weight-space.md), the coefficient determinant of $z_2,h_1$ is $-q[2]-q^{-2}=-[3]\ne0$. The extreme [weight spaces](../../../../../../weight-space.md) are spanned by $z_0,z_3$. Hence these six vectors form a [basis](../../../../../../basis.md) of the entire [tensor product of modules](../../../../../../tensor-product-of-modules.md). Each summand is a [simple module](../../../../../../irreducible-module.md): projecting a nonzero vector onto one of its distinct $K$ [weight spaces](../../../../../../weight-space.md) and applying the nonzero raising and lowering coefficients recovers its entire [basis](../../../../../../basis.md). Consequently

$$
\boxed{V_{1,1}\otimes V_{1,2}=W_3\oplus W_1\cong V_{1,3}\oplus V_{1,1}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
