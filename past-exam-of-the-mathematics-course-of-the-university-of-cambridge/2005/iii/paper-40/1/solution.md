<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Introduce nonnegative [slack variables](../../../../../slack-variable.md) $s_1,\ldots,s_4$ and write $z$ for the objective value. The initial [simplex dictionary](../../../../../simplex-dictionary.md), recovered from the original PDF rather than the corrupted converted table, is

$$
\begin{aligned}
s_1&=-10+x_1-2x_2+6x_3,\\
s_2&=6-x_2-2x_3,\\
s_3&=19-2x_1-10x_3,\\
s_4&=-2+x_1-x_2,\\
z&=2x_1+15x_2+18x_3.
\end{aligned}
$$

For this minimization convention, nonnegative objective coefficients give [dual feasibility](../../../../../dual-feasibility.md). The [dual simplex algorithm](../../../../../dual-simplex-algorithm.md) repairs a negative basic value while retaining those nonnegative [reduced costs](../../../../../reduced-cost.md). If the leaving row is $x_B=b+\sum_j a_jx_j$, $b<0$, an entering variable must have $a_j>0$; choose the smallest ratio of its objective coefficient to $a_j$.

Choose $s_1$ to leave. Eligible columns are $x_1,x_3$, with ratios $2/1=2$ and $18/6=3$. Thus $x_1$ enters. Solving its row and substituting gives

$$
\begin{aligned}
x_1&=10+s_1+2x_2-6x_3,\\
s_2&=6-x_2-2x_3,\\
s_3&=-1-2s_1-4x_2+2x_3,\\
s_4&=8+s_1+x_2-6x_3,\\
z&=20+2s_1+19x_2+6x_3.
\end{aligned}
$$

Now only $s_3$ has a negative basic value. Its only eligible entering column is $x_3$, so pivot there, with $s_3$ leaving. The resulting dictionary is

$$
\begin{aligned}
x_1&=7-5s_1-10x_2-3s_3,\\
x_3&=\tfrac12+s_1+2x_2+\tfrac12s_3,\\
s_2&=5-2s_1-5x_2-s_3,\\
s_4&=5-5s_1-11x_2-3s_3,\\
z&=23+8s_1+31x_2+3s_3.
\end{aligned}
$$

Setting the nonbasic variables $s_1,x_2,s_3$ to zero gives a [basic feasible solution](../../../../../basic-feasible-solution.md). The final objective row also proves $z\geq23$ for every [feasible point](../../../../../feasible-point.md), because its nonbasic variables are nonnegative. Hence the unique relaxed optimum is

$$
\boxed{(x_1,x_2,x_3)=(7,0,\tfrac12),\qquad z_{\mathrm{LP}}=23}.
$$

For the [integer program](../../../../../integer-programming.md), all four original [slack variables](../../../../../slack-variable.md) are [integers](../../../../../integer.md) whenever the decision variables are [integers](../../../../../integer.md). The fractional row can be written

$$
x_3-s_1-2x_2-\tfrac12s_3=\tfrac12.
$$

The [Gomory fractional cut](../../../../../gomory-fractional-cut.md) keeps the [fractional parts](../../../../../fractional-part.md) of these coefficients: $\{-1\}=\{-2\}=0$ and $\{-1/2\}=1/2$. It therefore gives $\tfrac12s_3\geq\tfrac12$, or $s_3\geq1$. Its validity can also be seen directly: the displayed row makes $s_3$ an odd nonnegative [integer](../../../../../integer.md). In original variables this cut is $2x_1+10x_3\leq18$.

Introduce the new integer-valued slack $u=s_3-1\geq0$, with initial row $u=-1+s_3$. It is primal infeasible but retains [dual feasibility](../../../../../dual-feasibility.md), so one more dual-simplex pivot has $u$ leave and $s_3$ enter. Substitute $s_3=1+u$ to obtain

$$
\begin{aligned}
x_1&=4-5s_1-10x_2-3u,\\
x_3&=1+s_1+2x_2+\tfrac12u,\\
s_2&=4-2s_1-5x_2-u,\\
s_4&=2-5s_1-11x_2-3u,\\
z&=26+8s_1+31x_2+3u.
\end{aligned}
$$

All basic values at $s_1=x_2=u=0$ are nonnegative [integers](../../../../../integer.md), including $s_3=1$. The objective row proves a lower bound of $26$ on every point satisfying the valid cut, hence on every integer-feasible point. It is attained at

$$
\boxed{(x_1,x_2,x_3)=(4,0,1),\qquad z_{\mathrm{IP}}=26}.
$$

The strictly positive nonbasic objective coefficients also show uniqueness. One Gomory cut and its reoptimization are sufficient.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
