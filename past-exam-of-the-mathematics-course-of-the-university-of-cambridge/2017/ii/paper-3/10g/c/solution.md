<h1 id="10g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the periodic [continued fraction](../../../../../../continued-fraction.md) $\sqrt d=[a_0;\overline{a_1,\ldots,a_m}]$. A direct [matrix](../../../../../../matrix.md) argument avoids any assumption about the parity of the period. Let

$$
 T(a)=\begin{pmatrix}a&1\\1&0\end{pmatrix},\quad
 M=T(a_1)\cdots T(a_m),\quad B=T(a_0),\quad N=BMB^{-1}.
$$

Periodicity says that $M$ fixes $\theta_1$ as a [Möbius transformation](../../../../../../mobius-transformation.md), while $B$ takes $\theta_1$ to $\sqrt d$. Thus $N=\begin{pmatrix}A&B_1\\C&D\end{pmatrix}$ has [integer](../../../../../../integer.md) entries and fixes $\sqrt d$. Equating rational and irrational parts in $A\sqrt d+B_1=\sqrt d(C\sqrt d+D)$ gives $A=D,B_1=dC$. Consequently

$$
 A^2-dC^2=\det N=(-1)^m.
$$

The [eigenvalue](../../../../../../eigenvalue.md) of $M$ on $(\theta_1,1)^T$ is its denominator $M_{21}\theta_1+M_{22}>1$; this uses $a_i\geq1$ and $\theta_1>1$, including the one-term period. The corresponding [eigenvalue](../../../../../../eigenvalue.md) of $N$ is $A+C\sqrt d>1$. If the [algebraic norm](../../../../../../algebraic-norm.md) is $-1$, square this unit; otherwise keep it. In either case there is a unit $u=X+Y\sqrt d>1$ of [algebraic norm](../../../../../../algebraic-norm.md) $1$ with [integer](../../../../../../integer.md) $X,Y$. Its powers have [integer](../../../../../../integer.md) coefficients and [algebraic norm](../../../../../../algebraic-norm.md) $1$, and are distinct since $u^j$ strictly increases. Hence **Pell's equation has infinitely many [integer](../../../../../../integer.md) solutions**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10G](../../10g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
