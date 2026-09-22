<h1 id="33b/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take

$$
I_0=[x_0,x_2],\qquad I_1=[x_2,x_1],\qquad I_2=[x_1,x_3].
$$

Now

$$
I_0\longrightarrow I_2,\qquad
I_1\longrightarrow I_1,I_2,\qquad
I_2\longrightarrow I_0,
$$

so

$$
A=\begin{pmatrix}0&0&1\\0&1&1\\1&0&0\end{pmatrix}.
$$

The recurrent pieces of this [covering graph](../../../../../../../directed-covering-graph-of-an-interval-map.md) are the two-cycle $I_0\leftrightarrow I_2$ and the loop at $I_1$; neither contains two competing closed routes. Also

$$
\operatorname{tr}(A^3)=\operatorname{tr}A=1,
$$

so this ordering forces no 3-cycle.

The bound is attained by the [piecewise linear function](../../../../../../../piecewise-linear-function.md)

$$
F(x)=
\begin{cases}
x+\dfrac23,&0\leq x\leq\dfrac13,\\[3pt]
\dfrac53-2x,&\dfrac13\leq x\leq\dfrac23,\\[3pt]
1-x,&\dfrac23\leq x\leq1.
\end{cases}
$$

Indeed,

$$
0\mapsto\frac23\mapsto\frac13\mapsto1\mapsto0
$$

is a 4-cycle with the required spatial order. On $I_0\cup I_2$, the fourth iterate is the [identity function](../../../../../../../identity-function.md). Within $I_1$, the fixed point is $5/9$ and

$$
F(x)-\frac59=-2\left(x-\frac59\right),
$$

so every other point eventually leaves $I_1$ and enters $I_0\cup I_2$. The map therefore has no horseshoe in any iterate and is not [chaotic](../../../../../../../glendinning-chaos.md). The minimum number of distinct 3-cycles is consequently $\boxed0$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [33B](../../../33b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
