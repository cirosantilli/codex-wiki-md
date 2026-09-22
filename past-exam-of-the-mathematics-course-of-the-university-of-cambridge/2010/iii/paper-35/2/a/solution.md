<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce nonnegative [slack variables](../../../../../../slack-variable.md) $s_1,s_2$ and let $z$ denote profit. We display each [simplex tableau](../../../../../../simplex-tableau.md) as coefficients of its row equation, with the coefficient of $z$ in the objective equation implicitly one. Thus a negative coefficient in the last row permits an improving entering variable. The initial [simplex tableau](../../../../../../simplex-tableau.md) is

$$
\begin{array}{c|rrrr|r}
\text{basis}&x_1&x_2&s_1&s_2&\text{RHS}\\\hline
s_1&1&2&1&0&6\\
s_2&2&1&0&1&6\\\hline
z&-3&-4&0&0&0
\end{array}.
$$

Use the [simplex method](../../../../../../simplex-method.md) with $x_2$ entering. The [simplex ratio test](../../../../../../simplex-ratio-test.md) gives ratios $6/2=3$ and $6/1=6$, so $s_1$ leaves. Divide its row by two and eliminate the other $x_2$ entries:

$$
\begin{array}{c|rrrr|r}
\text{basis}&x_1&x_2&s_1&s_2&\text{RHS}\\\hline
x_2&1/2&1&1/2&0&3\\
s_2&3/2&0&-1/2&1&3\\\hline
z&-1&0&2&0&12
\end{array}.
$$

Next $x_1$ enters. The positive-column ratios are $3/(1/2)=6$ and $3/(3/2)=2$, so $s_2$ leaves. After this pivot and a row reordering,

$$
\begin{array}{c|rrrr|r}
\text{basis}&x_1&x_2&s_1&s_2&\text{RHS}\\\hline
x_1&1&0&-1/3&2/3&2\\
x_2&0&1&2/3&-1/3&2\\\hline
z&0&0&5/3&2/3&14
\end{array}.
$$

The last row is $z=14-(5/3)s_1-(2/3)s_2$, so every nonnegative feasible solution has $z\leq14$. Setting the nonbasic variables to zero gives

$$
\boxed{x_1=x_2=2,\qquad z_{\max}=14.}
$$

The equality certificate also shows uniqueness, since both nonbasic objective coefficients are strictly unfavorable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
