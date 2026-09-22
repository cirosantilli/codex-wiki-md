<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Introduce integer-valued [slack variables](../../../../../slack-variable.md) $s_1=11-2x_1-x_2$ and $s_2=6+x_1-2x_2$. Write $Z=4x_1+3x_2$. The initial [simplex dictionary](../../../../../simplex-dictionary.md) is

$$
x_1,x_2\geq0,\qquad s_1=11-2x_1-x_2,\quad s_2=6+x_1-2x_2,\quad Z=4x_1+3x_2.
$$

In the [simplex algorithm](../../../../../simplex-algorithm.md), let $x_1$ enter. The first constraint is the only limiting one, so $s_1$ leaves at $x_1=11/2$. Substitution gives

$$
x_1=\frac{11}2-\frac12x_2-\frac12s_1,\quad s_2=\frac{23}2-\frac52x_2-\frac12s_1,\quad Z=22+x_2-2s_1.
$$

Now $x_2$ enters and $s_2$ leaves: its ratio $23/5$ is smaller than the first row's ratio $11$. The resulting [simplex dictionary](../../../../../simplex-dictionary.md) is

$$
\begin{aligned}
x_1&=\frac{16}5-\frac25s_1+\frac15s_2,\\
x_2&=\frac{23}5-\frac15s_1-\frac25s_2,\\
Z&=\frac{133}5-\frac{11}5s_1-\frac25s_2.
\end{aligned}
$$

All nonbasic objective coefficients are nonpositive, and the basic values are nonnegative. Thus **the continuous [linear program](../../../../../linear-programming.md) has optimum**

$$
\boxed{(x_1,x_2)=\left(\frac{16}5,\frac{23}5\right),\qquad Z=\frac{133}5.}
$$

For [integer programming](../../../../../integer-programming.md), a row $x_B+\sum_j a_jx_j=b$ with integer variables yields the [Gomory fractional cut](../../../../../gomory-fractional-cut.md) $\sum_j\{a_j\}x_j\geq\{b\}$, where $\{u\}=u-\lfloor u\rfloor$ is the [fractional part](../../../../../fractional-part.md). In the first row, the coefficient of $s_2$ on the left is $-1/5$, whose [fractional part](../../../../../fractional-part.md) is $4/5$, not $-1/5$. The two possible initial [Gomory fractional cuts](../../../../../gomory-fractional-cut.md) are therefore

$$
\begin{array}{c|c|c}
\text{row}&\text{cut in slacks}&\text{cut in original variables}\\\hline
x_1&\frac25s_1+\frac45s_2\geq\frac15&x_2\leq\frac92\\
x_2&\frac15s_1+\frac25s_2\geq\frac35&x_2\leq4.
\end{array}
$$

Indeed $s_1+2s_2=23-5x_2$. **Choose the second row:** $x_2\leq4$ implies $x_2\leq9/2$, so its cut removes a strictly larger portion of the feasible polygon. This compares both printed alternatives before any further integer rounding.

Use the normalized integer [slack variable](../../../../../slack-variable.md) $s_3=4-x_2$, rather than an unnecessarily scaled cut slack. At the current basis,

$$
s_3=-\frac35+\frac15s_1+\frac25s_2.
$$

The [simplex dictionary](../../../../../simplex-dictionary.md) is dual feasible but primal infeasible. In the [dual simplex algorithm](../../../../../dual-simplex-algorithm.md), $s_3$ leaves; the ratios of objective loss to improvement of this negative basic value are $11$ for $s_1$ and $1$ for $s_2$, so $s_2$ enters. The pivot gives

$$
\begin{aligned}
s_2&=\frac32-\frac12s_1+\frac52s_3,\\
x_1&=\frac72-\frac12s_1+\frac12s_3,\\
x_2&=4-s_3,\\
Z&=26-2s_1-s_3.
\end{aligned}
$$

The relaxed optimum is now $(7/2,4)$, still nonintegral. The fractional $x_1$ row gives the next [Gomory fractional cut](../../../../../gomory-fractional-cut.md)

$$
\frac12s_1+\frac12s_3\geq\frac12\quad\Longleftrightarrow\quad s_1+s_3\geq1\quad\Longleftrightarrow\quad x_1+x_2\leq7.
$$

The negative left-hand coefficient $-1/2$ of $s_3$ also has [fractional part](../../../../../fractional-part.md) $1/2$. Normalize the new integer [slack variable](../../../../../slack-variable.md) as $s_4=7-x_1-x_2$. Its dictionary row is $s_4=-1/2+s_1/2+s_3/2$. The [dual simplex algorithm](../../../../../dual-simplex-algorithm.md) chooses $s_3$ to enter: its ratio is $1/(1/2)=2$, compared with $2/(1/2)=4$ for $s_1$. Substitution gives

$$
\begin{aligned}
s_3&=1-s_1+2s_4,\\
s_2&=4-3s_1+5s_4,\\
x_1&=4-s_1+s_4,\\
x_2&=3+s_1-2s_4,\\
Z&=25-s_1-2s_4.
\end{aligned}
$$

Setting the nonbasic $s_1,s_4$ to zero gives a feasible integer solution. The final objective row bounds every point in the cut relaxation by $25$, so **the integer optimum is**

$$
\boxed{(x_1,x_2)=(4,3),\qquad Z=25.}
$$

Both cuts are valid for every original integer feasible point, making this also a certificate for the original [integer program](../../../../../integer-programming.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 212](../../paper-212-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
