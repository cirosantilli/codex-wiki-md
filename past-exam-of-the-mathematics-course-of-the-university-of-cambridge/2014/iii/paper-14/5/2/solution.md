<h1 id="5/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Both relators have zero exponent sums, so [abelianization](../../../../../../abelianization.md) gives $H_1(Y)=\mathbb Z^3$, with meridian variables $x,y,z$ corresponding to $a,b,c$. The [universal abelian cover](../../../../../../universal-abelian-cover.md) has [deck transformation group](../../../../../../deck-transformation-group.md) $\mathbb Z^3$ and coefficient [group ring](../../../../../../group-ring.md)

$$
R=\mathbb Z[x^{\pm1},y^{\pm1},z^{\pm1}].
$$

The [generalized Heegaard diagram](../../../../../../generalized-heegaard-diagram.md) gives a two-dimensional spine with one vertex, three edges and two faces. Its lifted [cellular chain complex](../../../../../../cellular-chain-complex.md) is

$$
0\longrightarrow R^2\xrightarrow{d_2}R^3\xrightarrow{d_1}R\longrightarrow0,
$$

where chosen lifts of the cells give

$$
d_1=\begin{pmatrix}x-1&y-1&z-1\end{pmatrix},\qquad
d_2=\begin{pmatrix}
1-yz&1-z\\
x-1&x(1-z)\\
y(x-1)&xy-1
\end{pmatrix}.
$$

The two columns are the abelianized [Fox derivatives](../../../../../../fox-derivative.md) of $[a,bc]$ and $[ab,c]$. The [Fox calculus](../../../../../../fox-calculus.md) identity gives $d_1d_2=0$; this can also be checked by multiplying the displayed matrices. There is no three-cell in this spine. One may use the lifted spine because its [deformation retraction](../../../../../../deformation-retraction.md) from $Y$ lifts to the [universal abelian cover](../../../../../../universal-abelian-cover.md).

The maximal minors of the [Alexander matrix](../../../../../../alexander-matrix.md), in row-pair order $(1,2),(1,3),(2,3)$, are

$$
(z-1)(xyz-1),\quad -(y-1)(xyz-1),\quad (x-1)(xyz-1).
$$

Their [greatest common divisor](../../../../../../greatest-common-divisor.md) in $R$ is $xyz-1$, since $x-1,y-1,z-1$ have no common nonunit divisor. Accordingly the [multivariable Alexander polynomial](../../../../../../multivariable-alexander-polynomial.md) is

$$
\boxed{\Delta_L(x,y,z)\doteq xyz-1.}
$$

The allowed units are $\pm x^iy^jz^k$. The single-variable specialization convention can introduce extra $(t-1)$ factors; the answer here is the genuinely [multivariable Alexander polynomial](../../../../../../multivariable-alexander-polynomial.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [5](../../5.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
