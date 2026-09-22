<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $A=k[x,y]$, $X=\operatorname{Spec}A$, and $U=X\setminus Z$. Since $A$ is an [integral domain](../../../../../../integral-domain.md), no nonzero global section is supported only at the origin, so

$$
H_Z^0(X,\mathcal O_X)=0.
$$

The [punctured affine plane](../../../../../../punctured-affine-plane.md) has the affine cover $U=D(x)\cup D(y)$. Its [Čech cochain complex](../../../../../../cech-cochain-complex.md) for the structure sheaf is

$$
0\longrightarrow A_x\oplus A_y
\xrightarrow{(a,b)\mapsto a-b}A_{xy}\longrightarrow0.
$$

Consequently

$$
H^0(U,\mathcal O_U)=A,
\qquad
H^1(U,\mathcal O_U)=\frac{A_{xy}}{A_x+A_y},
\qquad
H^i(U,\mathcal O_U)=0\quad(i\geq2).
$$

Because $X$ is affine, the higher [sheaf cohomology](../../../../../../sheaf-cohomology.md) of $\mathcal O_X$ vanishes. The [long exact sequence for local cohomology](../../../../../../long-exact-sequence-for-local-cohomology.md) therefore gives

$$
H_Z^1(X,\mathcal O_X)=0,
\qquad
H_Z^2(X,\mathcal O_X)
\cong\frac{k[x^{\pm1},y^{\pm1}]}{k[x^{\pm1},y]+k[x,y^{\pm1}]},
$$

and $H_Z^i(X,\mathcal O_X)=0$ for $i\geq3$. The nonzero group has the $k$-basis

$$
\{x^{-a}y^{-b}:a,b\geq1\}.
$$

This computes the [local cohomology of the affine plane supported at the origin](../../../../../../local-cohomology-of-the-affine-plane-supported-at-the-origin.md) in every degree.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
