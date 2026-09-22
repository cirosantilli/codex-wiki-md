<h1 id="20c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use payoff $P=-(2x_1-3x_2-2x_3)$, so maximization of $P$ is equivalent to the required minimization. In the given [simplex tableau](../../../../../../simplex-tableau.md), $x_1$ can increase the payoff. The [simplex ratio test](../../../../../../simplex-ratio-test.md) has candidate ratios $3/6=1/2$ in the $z_2$ row and $15/1=15$ in the $z_3$ row; the negative coefficient in the $x_2$ row imposes no upper bound. Thus $x_1$ enters the [simplex basis](../../../../../../simplex-basis.md) and $z_2$ leaves.

Divide the pivot row by $6$, then eliminate $x_1$ from the other rows. The resulting [simplex dictionary](../../../../../../simplex-dictionary.md) is

$$
\begin{aligned}
x_1-\tfrac32x_3-\tfrac16z_1+\tfrac16z_2&=\tfrac12,\\
x_2+\tfrac12x_3+\tfrac13z_1+\tfrac16z_2&=3,\\
z_3+10x_3+\tfrac{13}6z_1-\tfrac16z_2&=\tfrac{29}2,\\
P+\tfrac52x_3+\tfrac43z_1+\tfrac16z_2&=8.
\end{aligned}
$$

All [slack variables](../../../../../../slack-variable.md) and original variables are nonnegative. The last row therefore proves $P\le8$ for every [feasible point](../../../../../../feasible-point.md); setting the nonbasic variables $x_3,z_1,z_2$ to zero attains it and leaves all basic variables nonnegative. Hence

$$
\boxed{(x_1,x_2,x_3)=(\tfrac12,3,0),\qquad\min(2x_1-3x_2-2x_3)=-8.}
$$

The slack vector is $(0,0,29/2)$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [20C](../../20c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
