<h1 id="21h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Introduce slack variables $s_1,s_2,s_3\geq0$ after rewriting the third inequality as $x_1-x_2+x_3\leq2$. The initial dictionary is

$$
\begin{aligned}
s_1&=14-x_1-3x_2-x_3,\\
s_2&=5-4x_1-3x_2-2x_3,\\
s_3&=2-x_1+x_2-x_3,\\
z&=4x_1+3x_2+7x_3.
\end{aligned}
$$

In the [simplex method](../../../../../../simplex-method.md), $x_3$ enters first because it has the largest positive objective coefficient. The ratio test makes $s_3$ leave, and substitution gives

$$
\begin{aligned}
x_3&=2-x_1+x_2-s_3,\\
s_1&=12-4x_2+s_3,\\
s_2&=1-2x_1-5x_2+2s_3,\\
z&=14-3x_1+10x_2-7s_3.
\end{aligned}
$$

Next $x_2$ enters and $s_2$ leaves. Solving for $x_2$ produces the final objective row

$$
z=16-7x_1-3s_3-2s_2.
$$

All reduced costs are now nonpositive, so the dictionary is optimal at the nonbasic values $x_1=s_2=s_3=0$. Therefore

$$
\boxed{(x_1,x_2,x_3)=\left(0,\frac15,\frac{11}{5}\right),
\qquad z_{\max}=16}.
$$

The first constraint has slack $s_1=56/5$, while the second and third constraints are active.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
