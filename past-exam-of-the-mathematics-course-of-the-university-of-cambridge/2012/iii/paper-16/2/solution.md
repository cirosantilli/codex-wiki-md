<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Number the seven crossings from top to bottom. Orient the strand entering the top-left arch downward. With the usual positive braid crossing convention, the crossing signs are

$$
(+,+,+,-,-,+,+).
$$

To make the diagram calculation reproducible, its oriented [Gauss code](../../../../../gauss-code.md) is

$$
1_o\,2_u\,3_o\,6_u\,7_o\,1_u\,2_o\,4_u\,5_o\,7_u\,6_o\,5_u\,4_o\,3_u.
$$

Subscripts record overpassing and underpassing. In this convention a positive [trefoil knot](../../../../../trefoil-knot.md) has [knot signature](../../../../../signature-of-a-knot.md) $-2$.

Label the seven [Wirtinger generators](../../../../../wirtinger-generator.md) $x_0,\ldots,x_6$ successively between undercrossings, beginning just before the encounter $2_u$. The [Alexander matrix](../../../../../alexander-matrix.md), with rows ordered by crossing number, is

$$
M(t)=
\begin{pmatrix}
1-t&0&t&-1&0&0&0\\
t&-1&0&1-t&0&0&0\\
-1&1-t&0&0&0&0&t\\
0&0&0&1&-t&0&t-1\\
0&0&0&0&t-1&1&-t\\
0&t&-1&0&0&1-t&0\\
0&0&1-t&0&t&-1&0
\end{pmatrix}.
$$

At a positive crossing the [Fox derivative](../../../../../fox-derivative.md) entries at the overpassing, incoming and outgoing arcs are $1-t,t,-1$; at a negative crossing a unit multiple of the row has entries $t-1,1,-t$. Deleting the last row and column gives [determinant](../../../../../determinant.md) $t(t^4-5t^3+7t^2-5t+1)$. Hence a symmetric normalization of the **Alexander polynomial of a knot** is

$$
\boxed{\Delta_K(t)=t^2-5t+7-5t^{-1}+t^{-2}.}
$$

In particular, $\Delta_K(1)=-1$ in this displayed normalization; multiplying by $-1$ gives normalization $1$ and does not change any conclusion.

The [Seifert algorithm](../../../../../seifert-algorithm.md) produces four [Seifert circles](../../../../../seifert-circle.md) and seven bands. Its connected [Seifert surface](../../../../../seifert-surface.md) has [Euler characteristic](../../../../../euler-characteristic.md) $4-7=-3$, and so [genus](../../../../../genus-of-a-surface.md) $(1-(-3))/2=2$. Conversely, the [Alexander breadth bound on Seifert genus](../../../../../alexander-breadth-bound-on-seifert-genus.md) gives $2g_s(K)\geq4$. Therefore

$$
\boxed{g_s(K)=2.}
$$

For the [knot signature](../../../../../signature-of-a-knot.md), use the [alternating diagram signature formula](../../../../../alternating-diagram-signature-formula.md): for a reduced [alternating knot diagram](../../../../../alternating-knot-diagram.md),

$$
\sigma(K)=s_A(D)-c_+(D)-1,
$$

where $s_A$ counts circles in the all-$A$ bracket smoothing and $c_+$ counts positive crossings. Here the all-$A$ smoothing has four circles, the all-$B$ smoothing has five, and $c_+=5$. Thus

$$
\boxed{\sigma(K)=-2.}
$$

The opposite global [knot signature](../../../../../signature-of-a-knot.md) convention gives $+2$ instead.

For the [slice genus](../../../../../slice-genus.md), the [Levine-Tristram signature bound on the slice genus](../../../../../levine-tristram-signature-bound-on-the-slice-genus.md) at $-1$ gives $g_4(K)\geq1$. There is also an explicit [unknotting crossing](../../../../../unknotting-crossing.md): switch crossing $3$. A type III [Reidemeister move](../../../../../reidemeister-move.md) across the triangle formed by crossings $1,2,3$ makes crossing $3$ a removable kink. Next cancel pairs $(1,4)$ and $(2,5)$ by type II [Reidemeister moves](../../../../../reidemeister-move.md); crossings $7$ and $6$ then become removable kinks. This leaves the [unknot](../../../../../unknot.md). One [crossing change](../../../../../crossing-change.md) gives a genus-one [knot cobordism](../../../../../knot-cobordism.md) to the [unknot](../../../../../unknot.md): its movie consists of two oriented band moves, and capping the final [unknot](../../../../../unknot.md) by a disk in $B^4$ gives a surface of [genus](../../../../../genus-of-a-surface.md) one. Consequently

$$
\boxed{g_4(K)=1.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
