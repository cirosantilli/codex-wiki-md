<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a smooth complex [vector bundle](../../../../../vector-bundle.md) $E$, a connection is a complex-linear map $D:\Gamma(E)\to A^1(M;E)$ satisfying $D(fs)=df\otimes s+fDs$ for smooth complex functions $f$. Local trivializations supply flat local connections. A locally finite smooth [partition of unity](../../../../../partition-of-unity.md) $(\rho_i)$ subordinate to them gives $D=\sum_i\rho_iD_i$; local finiteness makes the sum smooth and $\sum_i\rho_i=1$ gives the [Leibniz rule](../../../../../leibniz-rule.md). Thus [connections on a vector bundle](../../../../../connection-vector-bundle.md) always exist on the usual paracompact smooth manifold.

Extend $D$ to bundle-valued forms by $D(\alpha\otimes s)=d\alpha\otimes s+(-1)^{\deg\alpha}\alpha\wedge Ds$. Squaring shows that $D^2(fs)=fD^2s$, so the [curvature form](../../../../../curvature-form.md) is the endomorphism-valued two-form $\Theta=D^2$. With a row frame $e=(e_1,\ldots,e_r)$, write $De=eA$; for coefficient columns $s=ev$, $Ds=e(dv+Av)$. Applying $D$ again and using the graded [Leibniz rule](../../../../../leibniz-rule.md) gives

$$
D^2(ev)=e(dA+A\wedge A)v.
$$

The cross terms $-A\wedge dv$ and $A\wedge dv$ cancel. Hence the [Cartan curvature matrix equation](../../../../../cartan-curvature-matrix-equation.md) in this convention is

$$
\boxed{\Theta=dA+A\wedge A.}
$$

For a frame change $e'=eg$, the [connection matrix](../../../../../connection-one-form.md) and curvature transform as $A'=g^{-1}Ag+g^{-1}dg$ and $\Theta'=g^{-1}\Theta g$. Trace is invariant under conjugation, so the local forms $\operatorname{Tr}\Theta$ patch into the global [trace of vector-bundle curvature](../../../../../trace-of-vector-bundle-curvature.md).

The induced [determinant connection](../../../../../determinant-connection.md) on $\det E=\Lambda^rE$ is

$$
D_r(s_1\wedge\cdots\wedge s_r)=\sum_{j=1}^r s_1\wedge\cdots\wedge Ds_j\wedge\cdots\wedge s_r,
$$

where the one-form factor of each $Ds_j$ is placed in front of the section factors. In the local determinant frame $e_1\wedge\cdots\wedge e_r$, only the diagonal terms survive, so its connection form is $\operatorname{Tr}A$. Its curvature is $d\operatorname{Tr}A$. Since

$$
\operatorname{Tr}(A\wedge A)=\sum_{i,j}A_{ij}\wedge A_{ji}=0
$$

by pairing off-diagonal terms and using $A_{ii}\wedge A_{ii}=0$, we obtain

$$
\boxed{\Theta_{D_r}=d\operatorname{Tr}A=\operatorname{Tr}\Theta_D.}
$$

It is closed locally by $d^2=0$, and thus closed globally.

For two connections, $B=D_1-D_0$ is a global endomorphism-valued one-form: the derivative terms cancel in their Leibniz rules. In a local frame $A_1=A_0+B$, so

$$
\Theta_1-\Theta_0=dB+A_0\wedge B+B\wedge A_0+B\wedge B.
$$

Taking traces cancels the mixed terms, because both factors are one-forms, and cancels $\operatorname{Tr}(B\wedge B)$. Therefore the [trace curvature transgression](../../../../../trace-curvature-transgression.md) formula is

$$
\boxed{\operatorname{Tr}\Theta_1-\operatorname{Tr}\Theta_0=d\operatorname{Tr}B.}
$$

The right-hand side is globally exact, proving independence of the [de Rham cohomology](../../../../../de-rham-cohomology.md) class without needing a sheaf-cohomology identification.

Finally let $e$ be a holomorphic frame for the [holomorphic line bundle](../../../../../holomorphic-line-bundle.md), with $h=\|e\|^2>0$. Define $De=e\,\partial\log h$, extending by the Leibniz rule. If $e'=eg$ for a nowhere-zero holomorphic function $g$, then $h'=|g|^2h$ and

$$
\partial\log h'=\partial\log h+g^{-1}dg.
$$

This is exactly the line-bundle frame-change law for a connection, so the local definitions glue globally. Its $(0,1)$ part is the [Dolbeault operator](../../../../../dolbeault-operator.md). Metric compatibility follows from $d\log h=\partial\log h+\bar\partial\log h$, or $dh=h(A+\overline A)$ for $A=\partial\log h$. These conditions uniquely force this $A$, identifying the [Chern connection](../../../../../chern-connection.md). Since a scalar one-form wedges with itself to zero,

$$
\boxed{\Theta=d(\partial\log h)=\bar\partial\partial\log h=-\partial\bar\partial\log h.}
$$

This agrees with the [local formula for the Chern connection on a line bundle](../../../../../local-formula-for-the-chern-connection-on-a-line-bundle.md); keeping the order of the two Dolbeault differentials fixes the sign.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
