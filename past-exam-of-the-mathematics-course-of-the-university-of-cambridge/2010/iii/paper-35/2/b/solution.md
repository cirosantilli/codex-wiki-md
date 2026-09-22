<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Add the [slack variable](../../../../../../slack-variable.md) $s_3$ for the forgotten constraint. In the optimal [simplex tableau](../../../../../../simplex-tableau.md) from part (a), $x_1+x_2=4-(s_1+s_2)/3$. Hence the new row in canonical form is

$$
s_3-\frac43s_1-\frac43s_2=-1.
$$

Appending it gives

$$
\begin{array}{c|rrrrr|r}
\text{basis}&x_1&x_2&s_1&s_2&s_3&\text{RHS}\\\hline
x_1&1&0&-1/3&2/3&0&2\\
x_2&0&1&2/3&-1/3&0&2\\
s_3&0&0&-4/3&-4/3&1&-1\\\hline
z&0&0&5/3&2/3&0&14
\end{array}.
$$

The objective row remains dual feasible, but $s_3=-1$ makes the basic solution infeasible. Apply the [dual simplex algorithm](../../../../../../dual-simplex-algorithm.md): $s_3$ leaves, and the eligible columns are $s_1,s_2$, whose negative coefficients can repair this row. The dual ratio test compares

$$
\frac{5/3}{4/3}=\frac54,\qquad \frac{2/3}{4/3}=\frac12.
$$

Thus $s_2$ enters. Pivoting on $-4/3$ and eliminating its column gives

$$
\begin{array}{c|rrrrr|r}
\text{basis}&x_1&x_2&s_1&s_2&s_3&\text{RHS}\\\hline
x_1&1&0&-1&0&1/2&3/2\\
x_2&0&1&1&0&-1/4&9/4\\
s_2&0&0&1&1&-3/4&3/4\\\hline
z&0&0&1&0&1/2&27/2
\end{array}.
$$

All basic values are nonnegative and the objective equation is $z=27/2-s_1-s_3/2$. Therefore

$$
\boxed{x_1=\frac32,\qquad x_2=\frac94,\qquad z_{\max}=\frac{27}{2},\qquad s_2=\frac34.}
$$

Both binding constraints have zero slack, and the final objective row proves global optimality. The two nonbasic penalties are strictly positive, so this optimum is unique.

## ↑ Ancestors (11)

1. [B](../b.md)
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
