<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the PDF's first constraint, $2x_1+x_2\geq6$; the TeX aid substitutes a different inequality. Introduce a surplus $x_3$, slacks $x_4,x_5$, and one artificial variable $x_6$, all nonnegative. The initial [simplex dictionary](../../../../../../simplex-dictionary.md) is

$$
x_6=6-2x_1-x_2+x_3,\qquad x_4=-2x_1+x_2,\qquad x_5=8-x_1-2x_2.
$$

The initial basis is $(x_6,x_4,x_5)$, with values $(6,0,8)$. In [two-phase simplex](../../../../../../two-phase-simplex.md), Phase I maximizes $w=-x_6=-6+2x_1+x_2-x_3$. We use the [Bland pivoting rule](../../../../../../bland-pivoting-rule.md): the smallest-index nonbasic variable with positive reduced cost enters, and among minimum-ratio ties the smallest-index basic variable leaves.

First $x_1$ enters. The ratios for $x_6,x_4,x_5$ are $3,0,8$, so $x_4$ leaves in a degenerate pivot. The resulting dictionary is

$$
x_1=\tfrac12x_2-\tfrac12x_4,\qquad x_6=6-2x_2+x_3+x_4,\qquad x_5=8-\tfrac52x_2+\tfrac12x_4,\qquad w=-6+2x_2-x_3-x_4.
$$

Next $x_2$ enters. It reduces $x_6$ and $x_5$ with ratios $3$ and $16/5$, while $x_1$ increases. Thus $x_6$ leaves. The Phase I maximum is $0$, with a feasible original basis; remove $x_6$ and obtain

$$
x_1=\tfrac32+\tfrac14x_3-\tfrac14x_4,\qquad x_2=3+\tfrac12x_3+\tfrac12x_4,\qquad x_5=\tfrac12-\tfrac54x_3-\tfrac34x_4.
$$

In Phase II the original objective is $z=21/2+(7/4)x_3+(5/4)x_4$. Bland's rule makes $x_3$ enter, and $x_5$ leaves at ratio $2/5$. This gives

$$
x_1=\tfrac85-\tfrac25x_4-\tfrac15x_5,\qquad x_2=\tfrac{16}5+\tfrac15x_4-\tfrac25x_5,\qquad x_3=\tfrac25-\tfrac35x_4-\tfrac45x_5,\qquad z=\tfrac{56}5+\tfrac15x_4-\tfrac75x_5.
$$

Finally $x_4$ enters. The decreasing basic variables $x_1,x_3$ have ratios $4$ and $2/3$, so $x_3$ leaves. The final tableau, with the basic columns suppressed, is

$$
\begin{array}{c|rr|r}
\text{row}&x_3&x_5&\text{right side}\\\hline
x_1&-2/3&-1/3&4/3\\
x_2&1/3&2/3&10/3\\
x_4&5/3&4/3&2/3\\\hline
z&1/3&5/3&34/3
\end{array}
$$

Each row means its row variable plus the displayed nonbasic terms equals the right side. Since $z=34/3-x_3/3-5x_5/3$, no nonnegative choice of nonbasic variables improves the objective. Thus

$$
\boxed{(x_1,x_2)=\left(\frac43,\frac{10}3\right),\qquad z^*=\frac{34}3.}
$$

The slacks are $x_3=x_5=0$, $x_4=2/3$.

A different entering rule is faster here. Selecting the largest eligible index in the initial Phase I objective makes $x_2$ enter and $x_5$ leave. The dictionary then has $x_6=2-(3/2)x_1+x_3+x_5/2$ and $x_4=4-(5/2)x_1-x_5/2$. Entering $x_1$ makes $x_6$ leave at $x_1=4/3$, directly reaching the final original basis $(x_1,x_2,x_4)$. Hence **two pivots suffice instead of Bland's four**, and Phase II needs no further pivot. This comparison concerns this instance, not a general superiority of that entering rule.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
