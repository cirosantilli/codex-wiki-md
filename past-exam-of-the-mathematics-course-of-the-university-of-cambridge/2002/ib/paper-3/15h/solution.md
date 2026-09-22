<h1 id="15h/solution">Solution</h1>

↑ **Parent:** [15H](../15h.md)

Introduce surplus variables $s_1,s_2$, slack $s_3$, and artificial variables $a_1,a_2$, all nonnegative. The [two-phase simplex](../../../../../two-phase-simplex.md) standard-form equations are

$$
x_1-x_2-s_1+a_1=1,\qquad
4x_1-x_2-s_2+a_2=10,\qquad x_2+s_3=6.
$$

Phase I maximizes $w=-a_1-a_2$. An initial [basic feasible solution](../../../../../basic-feasible-solution.md) has basic variables $(a_1,a_2,s_3)=(1,10,6)$ and all others zero. Its [simplex dictionary](../../../../../simplex-dictionary.md) is

$$
a_1=1-x_1+x_2+s_1,\qquad a_2=10-4x_1+x_2+s_2,\qquad s_3=6-x_2,
\qquad w=-11+5x_1-2x_2-s_1-s_2.
$$

Let $x_1$ enter. The [simplex ratio test](../../../../../simplex-ratio-test.md) gives $1$ from the $a_1$ row and $10/4$ from the $a_2$ row, so $a_1$ leaves. After this pivot,

$$
x_1=1+x_2+s_1-a_1,\quad a_2=6-3x_2-4s_1+4a_1+s_2,\quad s_3=6-x_2,
\quad w=-6+3x_2+4s_1-5a_1-s_2.
$$

Choose $x_2$ to enter; the limiting ratios are $6/3=2$ and $6$, so $a_2$ leaves. The resulting dictionary is

$$
\begin{aligned}
x_1&=3-\tfrac13s_1+\tfrac13s_2+\tfrac13a_1-\tfrac13a_2,\\
x_2&=2-\tfrac43s_1+\tfrac13s_2+\tfrac43a_1-\tfrac13a_2,\\
s_3&=4+\tfrac43s_1-\tfrac13s_2-\tfrac43a_1+\tfrac13a_2,\\
w&=-a_1-a_2.
\end{aligned}
$$

Thus $\boxed{w_{\max}=0}$, attained at $(x_1,x_2,s_3)=(3,2,4)$ with $s_1=s_2=a_1=a_2=0$. Since $w\le0$ for every feasible Phase I point, this proves feasibility and completes Phase I.

Delete the artificial variables and restore the original objective $z=-2x_1+3x_2$. The resulting Phase II dictionary is

$$
x_1=3-\tfrac13s_1+\tfrac13s_2,\quad x_2=2-\tfrac43s_1+\tfrac13s_2,
\quad s_3=4+\tfrac43s_1-\tfrac13s_2,\quad z=-\tfrac{10}3s_1+\tfrac13s_2.
$$

Let $s_2$ enter; only $s_3$ decreases, and it reaches zero at $s_2=12$. Pivoting gives

$$
\boxed{x_1=7+s_1-s_3,\quad x_2=6-s_3,\quad s_2=12+4s_1-3s_3,\quad z=4-2s_1-s_3}.
$$

An optimal [simplex tableau](../../../../../simplex-tableau.md), with each row recording its equality, is

$$
\begin{array}{c|rrrrr|r}
\text{basic}&x_1&x_2&s_1&s_2&s_3&\text{right side}\\\hline
x_1&1&0&-1&0&1&7\\
x_2&0&1&0&0&1&6\\
s_2&0&0&-4&1&3&12\\\hline
z&0&0&2&0&1&4
\end{array}.
$$

Both reduced costs in the maximization dictionary are negative. Setting nonbasic $s_1=s_3=0$ therefore gives

$$
\boxed{(x_1,x_2)=(7,6),\qquad z_{\max}=4}.
$$

As a direct optimality check, $x_1\ge1+x_2$ implies $z\le-2+x_2\le4$; the displayed point attains both equalities.

## ↑ Ancestors (10)

1. [15H](../15h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
