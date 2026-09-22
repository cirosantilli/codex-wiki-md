<h1 id="23g/solution">Solution</h1>

↑ **Parent:** [23G](../23g.md)

Use the original PDF: the objective is $z=-x_1+3x_2$, and the second constraint has coefficient $2$ on $x_2$. The TeX transcription corrupts both, as well as the nonnegativity condition. Introduce surplus variables $s_1,s_2$, slack variables $s_3,s_4$, and artificial variables $a_1,a_2$, all nonnegative. The [two-phase simplex](../../../../../two-phase-simplex.md) Phase One problem is

$$
\min w=a_1+a_2,
$$



$$
x_1+x_2-s_1+a_1=3,\quad -x_1+2x_2-s_2+a_2=6,\quad
-x_1+x_2+s_3=2,\quad x_2+s_4=5.
$$

The initial [basis](../../../../../basis.md) $(a_1,a_2,s_3,s_4)$ has values $(3,6,2,5)$, and its objective dictionary is $w=9-3x_2+s_1+s_2$. Enter $x_2$: the ratio test makes $s_3$ leave at $x_2=2$. The resulting dictionary includes

$$
x_2=2+x_1-s_3,\quad a_1=1-2x_1+s_1+s_3,\quad
 a_2=2-x_1+s_2+2s_3,\quad s_4=3-x_1+s_3,
$$

with $w=3-3x_1+s_1+s_2+3s_3$. Enter $x_1$ next; $a_1$ leaves at $x_1=1/2$. Now

$$
x_1=\frac12+\frac{s_1+s_3-a_1}{2},\quad
x_2=\frac52+\frac{s_1-s_3-a_1}{2},
$$



$$
a_2=\frac32-\frac{s_1}{2}+s_2+\frac{3s_3}{2}+\frac{a_1}{2},\quad
s_4=\frac52-\frac{s_1}{2}+\frac{s_3+a_1}{2},
$$

and $w=3/2-s_1/2+s_2+3s_3/2+3a_1/2$. Enter $s_1$; the ratio test makes $a_2$ leave at $s_1=3$. This produces $x_1=2$, $x_2=4$, $s_1=3$, $s_4=1$ with both artificial variables zero. Since $w\ge0$ always, **the Phase One minimum is zero**, proving feasibility and providing an original-variable [basis](../../../../../basis.md).

Delete the artificial columns. The starting Phase Two dictionary is

$$
x_1=2+s_2+2s_3,\quad x_2=4+s_2+s_3,\quad
s_1=3+2s_2+3s_3,\quad s_4=1-s_2-s_3,
$$



$$
z=10+2s_2+s_3.
$$

Enter $s_2$, whose reduced gain is positive. Only $s_4$ decreases, and it leaves at step one. Eliminating $s_2=1-s_3-s_4$ gives the optimal dictionary

$$
x_1=3+s_3-s_4,\quad x_2=5-s_4,\quad
s_1=5+s_3-2s_4,\quad s_2=1-s_3-s_4,\quad
z=12-s_3-2s_4.
$$

Equivalently, with row equations written as the displayed coefficients times the variables equal to the right-hand side, the optimal [simplex tableau](../../../../../simplex-tableau.md) is

$$
\begin{array}{c|rrrrrrr|r}
 &x_1&x_2&s_1&s_2&s_3&s_4&z&\mathrm{RHS}\\\hline
x_1&1&0&0&0&-1&1&0&3\\
x_2&0&1&0&0&0&1&0&5\\
s_1&0&0&1&0&-1&2&0&5\\
s_2&0&0&0&1&1&1&0&1\\\hline
z&0&0&0&0&1&2&1&12
\end{array}
$$

The objective row represents $z+s_3+2s_4=12$. Nonnegative nonbasic variables cannot improve the objective, so reading them as zero proves

$$
\boxed{(x_1,x_2)=(3,5),\qquad z_{\max}=12.}
$$

Both nonbasic reduced costs are strictly unfavorable, so this optimal point is unique.

## ↑ Ancestors (10)

1. [23G](../23g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
