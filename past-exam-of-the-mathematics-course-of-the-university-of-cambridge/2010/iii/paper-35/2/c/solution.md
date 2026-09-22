<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The old [slack variable](../../../../../../slack-variable.md) $s_3$ is exactly the amount now sold, so rename its column $y$. No further slack is added: the PDF specifies an equality. The feasible equations are otherwise unchanged. If $z_0$ is the old profit, the new profit is $z=z_0+y$. Substituting this into the old objective equation gives

$$
z+s_1-\frac12y=\frac{27}{2}.
$$

This is the [simplex objective update for a priced slack variable](../../../../../../simplex-objective-update-for-a-priced-slack-variable.md). The altered [simplex tableau](../../../../../../simplex-tableau.md) is

$$
\begin{array}{c|rrrrr|r}
\text{basis}&x_1&x_2&s_1&s_2&y&\text{RHS}\\\hline
x_1&1&0&-1&0&1/2&3/2\\
x_2&0&1&1&0&-1/4&9/4\\
s_2&0&0&1&1&-3/4&3/4\\\hline
z&0&0&1&0&-1/2&27/2
\end{array}.
$$

The coefficient $-1/2$ makes $y$ an improving entering variable. Its only positive constraint-row coefficient is $1/2$ in the $x_1$ row, whose ratio is $(3/2)/(1/2)=3$. Thus $x_1$ leaves. The [simplex method](../../../../../../simplex-method.md) pivot gives

$$
\begin{array}{c|rrrrr|r}
\text{basis}&x_1&x_2&s_1&s_2&y&\text{RHS}\\\hline
y&2&0&-2&0&1&3\\
x_2&1/2&1&1/2&0&0&3\\
s_2&3/2&0&-1/2&1&0&3\\\hline
z&1&0&0&0&0&15
\end{array}.
$$

The objective equation $z=15-x_1$ proves optimality. One optimal basic solution is

$$
\boxed{x_1=0,\qquad x_2=3,\qquad y=3,\qquad z_{\max}=15.}
$$

The zero reduced cost of $s_1$ permits alternative optima. In fact all optimal solutions are

$$
\boxed{x_1=0,\qquad 0\leq x_2\leq3,\qquad y=15-4x_2.}
$$

These satisfy both remaining inequalities, and the equality then makes their profit exactly fifteen.

## ↑ Ancestors (11)

1. [C](../c.md)
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
