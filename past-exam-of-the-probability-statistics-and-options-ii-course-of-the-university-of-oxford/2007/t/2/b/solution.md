<h1 id="t/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Introduce nonnegative [slack variables](../../../../../slack-variable.md) $s_1,s_2$ and use a [simplex tableau](../../../../../simplex-tableau.md) with the last row representing $z-c^{\mathsf T}x=0$. The starting tableau is

$$
\begin{array}{c|rrrrr|r}
&x_1&x_2&x_3&s_1&s_2&\text{RHS}\\\hline
s_1&2&3&5&1&0&33\\
s_2&1&2&3&0&1&18\\\hline
z&-3&-4&-8&0&0&0
\end{array}
$$

Enter $x_3$ and let $s_2$ leave. Dividing the second row by three and eliminating its column gives

$$
\begin{array}{c|rrrrr|r}
&x_1&x_2&x_3&s_1&s_2&\text{RHS}\\\hline
s_1&1/3&-1/3&0&1&-5/3&3\\
x_3&1/3&2/3&1&0&1/3&6\\\hline
z&-1/3&4/3&0&0&8/3&48
\end{array}.
$$

Enter $x_1$ and let $s_1$ leave. The next [simplex tableau](../../../../../simplex-tableau.md) is

$$
\begin{array}{c|rrrrr|r}
&x_1&x_2&x_3&s_1&s_2&\text{RHS}\\\hline
x_1&1&-1&0&3&-5&9\\
x_3&0&1&1&-1&2&3\\\hline
z&0&1&0&1&1&51
\end{array}.
$$

Thus

$$
\boxed{(x_1,x_2,x_3)=(9,0,3),\qquad z_{\max}=51.}
$$

The pivot choices and the optimality certificate are justified in the following parts.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [T](../../../t.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
