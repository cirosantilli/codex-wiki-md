<h1 id="20d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Continue the [simplex algorithm](../../../../../../simplex-algorithm.md) using dictionaries, with nonbasic variables zero at the current vertex. The given basis has payoff

$$
f=\frac{116}{9}+\frac{17}{9}x_2-\frac{121}{9}x_3-\frac49z_3.
$$

Thus $x_2$ enters. Its positive row coefficients give ratios $11$ for $z_1$ and $77/4$ for $z_2$; the $x_1$ row does not restrict this increase. Therefore $z_1$ leaves. After that pivot,

$$
\begin{aligned}x_2&=11+11x_3-z_1,\\z_2&=11-11x_3+\tfrac43z_1-\tfrac13z_3,\\x_1&=\tfrac{17}3+\tfrac43x_3-\tfrac29z_1-\tfrac19z_3,\\f&=\tfrac{101}3+\tfrac{22}3x_3-\tfrac{17}9z_1-\tfrac49z_3.\end{aligned}
$$

Now $x_3$ enters. Only the $z_2$ row decreases along this move, and its ratio is $11/11=1$, so $z_2$ leaves. The final dictionary is

$$
\boxed{\begin{aligned}x_1&=7-\tfrac2{33}z_1-\tfrac4{33}z_2-\tfrac5{33}z_3,\\x_2&=22+\tfrac13z_1-z_2-\tfrac13z_3,\\x_3&=1+\tfrac4{33}z_1-\tfrac1{11}z_2-\tfrac1{33}z_3,\\f&=41-z_1-\tfrac23z_2-\tfrac23z_3.\end{aligned}}
$$

All reduced payoff coefficients are nonpositive. Since the slacks must be nonnegative, $f\leq41$, attained with $z=0$. Hence $\boxed{x^*=(7,22,1),\quad f^*=41}$. Direct substitution makes all three original constraints equalities. The final dictionary is the optimal tableau expressed with basic variables on the left, not just a proposed feasible vertex.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20D](../../20d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
