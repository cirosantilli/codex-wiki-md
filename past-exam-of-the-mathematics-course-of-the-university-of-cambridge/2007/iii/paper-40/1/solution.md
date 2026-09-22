<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Introduce nonnegative [slack variables](../../../../../slack-variable.md) $s_1=2+x_1-x_2$, $s_2=8-x_1-2x_2$ and $s_3=8-2x_1-x_2$, and write the objective as $Z$. With $x_1,x_2$ nonbasic, the initial [simplex dictionary](../../../../../simplex-dictionary.md) is

$$
\begin{aligned}
s_1&=2+x_1-x_2,&s_2&=8-x_1-2x_2,\\
s_3&=8-2x_1-x_2,&Z&=x_1+x_2.
\end{aligned}
$$

This is feasible at the origin. Enter $x_1$. The [simplex ratio test](../../../../../simplex-ratio-test.md) selects $s_3$ to leave, since its bound is $x_1\leq4$, compared with $x_1\leq8$ from $s_2$. Pivoting gives

$$
\begin{aligned}
x_1&=4-\tfrac12x_2-\tfrac12s_3,\\
s_1&=6-\tfrac32x_2-\tfrac12s_3,\\
s_2&=4-\tfrac32x_2+\tfrac12s_3,\\
Z&=4+\tfrac12x_2-\tfrac12s_3.
\end{aligned}
$$

Now enter $x_2$. The ratio test chooses $s_2$ to leave: its bound $8/3$ is smaller than $4$ from $s_1$ and $8$ from $x_1$. The resulting dictionary is

$$
\begin{aligned}
x_1&=\tfrac83+\tfrac13s_2-\tfrac23s_3,\\
x_2&=\tfrac83-\tfrac23s_2+\tfrac13s_3,\\
s_1&=2+s_2-s_3,\\
Z&=\tfrac{16}3-\tfrac13s_2-\tfrac13s_3.
\end{aligned}
$$

All basic values are nonnegative and all nonbasic objective coefficients are nonpositive. The [simplex algorithm](../../../../../simplex-algorithm.md) therefore certifies

$$
\boxed{x_1=x_2=\frac83,\qquad Z_{\mathrm{LP}}=\frac{16}3.}
$$

The negative objective coefficients also make this continuous optimum unique.

For integer $x_1,x_2$, all three original slacks are integers. Apply a [Gomory fractional cut](../../../../../gomory-fractional-cut.md) to the row

$$
x_1-\tfrac13s_2+\tfrac23s_3=\tfrac83.
$$

The fractional part of $-1/3$ is $2/3$, so the cut is $\frac23s_2+\frac23s_3\geq\frac23$, or $s_2+s_3\geq1$. To justify it directly, rewrite the row as

$$
(x_1-s_2)+\tfrac23(s_2+s_3)=\tfrac83.
$$

The parenthesized term is an integer and is at most $8/3$, since the other term is nonnegative. It is therefore at most $2$, proving the cut. This retains every feasible integer solution and excludes the current fractional optimum. Since $s_2+s_3=16-3(x_1+x_2)$, the cut is equivalently $x_1+x_2\leq5$.

Introduce the integer-valued nonnegative slack $t=s_2+s_3-1$. Its dictionary row is $t=-1+s_2+s_3$, so primal feasibility fails while the objective row remains dual feasible. In the [dual simplex algorithm](../../../../../dual-simplex-algorithm.md), $t$ leaves; $s_2,s_3$ tie in the dual ratio test, each with ratio $1/3$. Choose $s_2$ to enter. Substituting $s_2=1+t-s_3$ gives

$$
\begin{aligned}
x_1&=3+\tfrac13t-s_3,&x_2&=2-\tfrac23t+s_3,\\
s_1&=3+t-2s_3,&s_2&=1+t-s_3,\\
Z&=5-\tfrac13t.
\end{aligned}
$$

This dictionary is feasible at $t=s_3=0$ and certifies the cut relaxation's optimum $Z=5$, achieved at the integer point $(3,2)$.

To find every optimal integer point, the objective row forces $t=0$. Nonnegativity of all the remaining rows then reduces to $0\leq s_3\leq1$. On this optimal edge, $(x_1,x_2)=(3-s_3,2+s_3)$. Since $s_3$ must be integral, only its two endpoints are possible:

$$
\boxed{(x_1,x_2)=(3,2)\text{ or }(2,3),\qquad Z_{\mathrm{IP}}=5.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
