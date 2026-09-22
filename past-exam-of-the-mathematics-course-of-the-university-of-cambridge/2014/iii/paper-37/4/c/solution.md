<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Introduce nonnegative surplus variables

$$
r_1=5x_1+6x_2+x_3-1,\quad r_2=7x_1+5x_2+x_3-1,\quad r_3=4x_1+3x_2+5x_3-1.
$$

At the proposed starting [basic feasible solution](../../../../../../basic-feasible-solution.md), the basic variables are $x_1,r_1,r_2$ and the nonbasic variables are $x_2,x_3,r_3$. Its [simplex dictionary](../../../../../../simplex-dictionary.md), with objective $z=x_1+x_2+x_3$, is

$$
\begin{aligned}
x_1&=(1-3x_2-5x_3+r_3)/4,\\
r_1&=(1+9x_2-21x_3+5r_3)/4,\\
r_2&=(3-x_2-31x_3+7r_3)/4,\\
z&=(1+x_2-x_3+r_3)/4.
\end{aligned}
$$

Increase $x_3$ to decrease $z$. The [simplex ratio test](../../../../../../simplex-ratio-test.md) gives limits $1/5$ from $x_1$, $1/21$ from $r_1$, and $3/31$ from $r_2$. The smallest is $1/21$, so $x_3$ enters and $r_1$ leaves. After this single pivot the dictionary is

$$
\begin{aligned}
x_1&=(4+5r_1-r_3-27x_2)/21,\\
x_3&=(1-4r_1+5r_3+9x_2)/21,\\
r_2&=(8+31r_1-2r_3-75x_2)/21,\\
z&=(5+r_1+4r_3+3x_2)/21.
\end{aligned}
$$

All objective coefficients of nonbasic variables are strictly positive. Thus the [simplex method](../../../../../../simplex-method.md) has reached its unique optimum:

$$
\boxed{x=(4/21,0,1/21),\qquad z=5/21.}
$$

The feasible dual vector $y=(1/21,0,4/21)$ has the same objective, providing an independent [weak duality](../../../../../../weak-duality.md) certificate. Normalization gives

$$
\boxed{p=(4/5,0,1/5),\qquad q=(1/5,0,4/5),\qquad v=21/5-5=-4/5.}
$$

These are all the equilibria: the dual's strict slack in row two forces $p_2=0$, and the primal's strict slack in column two forces $q_2=0$. Equality of the two active row and column payoffs then fixes the displayed [probabilities](../../../../../../probability.md). The value is the first player's expected net loss; the second gains $4/5$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
