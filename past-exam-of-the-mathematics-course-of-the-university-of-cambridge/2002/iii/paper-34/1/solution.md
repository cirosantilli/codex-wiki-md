<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Introduce the nonnegative [integer](../../../../../integer.md) [surplus variables](../../../../../surplus-variable.md) $z_1=3x_1+x_2-4$ and $z_2=x_1+2x_2-4$. Solving these two equalities gives the optimal relaxed [simplex dictionary](../../../../../simplex-dictionary.md)

$$
x_1=\frac45+\frac25z_1-\frac15z_2,\qquad
x_2=\frac85-\frac15z_1+\frac35z_2,
$$

with objective

$$
C=3x_1+4x_2=\frac{44}5+\frac25z_1+\frac95z_2.
$$

The printed tableau has a sign error in the first row: in equality-row form the coefficient of $z_2$ must be $+1/5$, rather than $-1/5$. The defining constraints and the printed objective row both confirm this correction. The second row, from which the required cut is obtained, is unaffected.

The [cutting-plane method](../../../../../cutting-plane-method.md) solves the [linear programming](../../../../../linear-programming.md) relaxation and, if the optimum is fractional, adds an inequality valid for every feasible [integer](../../../../../integer.md) point but violated by that optimum. For an all-[integer](../../../../../integer.md) tableau row

$$
x_B+\sum_j a_jz_j=b,
$$

write each coefficient as its [integer](../../../../../integer.md) part plus its [fractional part](../../../../../fractional-part.md). The quantity $x_B+\sum_j\lfloor a_j\rfloor z_j$ is an [integer](../../../../../integer.md), while $\sum_j\{a_j\}z_j$ is nonnegative. Thus the [integer](../../../../../integer.md) is at most $\lfloor b\rfloor$, and subtraction gives the [Gomory fractional cut](../../../../../gomory-fractional-cut.md)

$$
\sum_j\{a_j\}z_j\ge\{b\}.
$$

It retains every feasible [integer](../../../../../integer.md) point and cuts off the fractional basic point with all nonbasic $z_j=0$.

Apply this to the row $x_2+\frac15z_1-\frac35z_2=\frac85$. Since $\{1/5\}=1/5$, $\{-3/5\}=2/5$ and $\{8/5\}=3/5$, the resulting valid inequality is

$$
\boxed{\frac15z_1+\frac25z_2\ge\frac35.}
$$

Multiply by five and add an [integer](../../../../../integer.md) slack $w=z_1+2z_2-3\ge0$. Its row is $w-z_1-2z_2=-3$. At the old relaxed optimum, $w=-3$ is negative, while the minimization objective coefficients $2/5,9/5$ remain nonnegative. This is the starting configuration for the [dual simplex algorithm](../../../../../dual-simplex-algorithm.md): retain [dual feasibility](../../../../../dual-feasibility.md) and pivot to repair the negative basic value.

The cut row permits either $z_1$ or $z_2$ to enter. The dual ratio test gives

$$
\frac{2/5}{1}=\frac25,\qquad \frac{9/5}{2}=\frac9{10}.
$$

Thus $z_1$ enters and $w$ leaves. Solving the cut row and substituting gives

$$
\begin{aligned}
z_1&=3-2z_2+w,\\
x_1&=2-z_2+\frac25w,\\
x_2&=1+z_2-\frac15w,\\
C&=10+z_2+\frac25w.
\end{aligned}
$$

Setting the nonbasic variables $z_2=w=0$ gives nonnegative basic values $z_1=3,x_1=2,x_2=1$. The new objective coefficients are nonnegative, so this is optimal for the cut relaxation. Its decision variables are already [integer](../../../../../integer.md) and satisfy the original inequalities. Therefore

$$
\boxed{x_1=2,\qquad x_2=1,\qquad C_{\min}=10.}
$$

Indeed the positive coefficients of both nonbasic variables make this relaxed optimizer unique. No additional cut is needed.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
