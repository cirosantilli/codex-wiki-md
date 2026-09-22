<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For any feasible $x,y$, increasing $z$ lowers the objective, so the additional upper bound makes $z^*=0$. Feasibility then requires $2x-y\leq2$. The lowest feasible value of $y$ on the circle occurs at the lower intersection with $2x-y=2$. Solving gives the candidate

$$
x^*=\frac{4-\sqrt{21}}5,\qquad y^*=-\frac{2+2\sqrt{21}}5,\qquad z^*=0.
$$

A global certificate avoids relying on the circle sketch. Introduce [Lagrange multipliers](../../../../../../lagrange-multiplier.md) for $g\leq0$, $z\leq0$ and $h=0$:

$$
L=3y-z+\lambda g+\nu z+\mu h.
$$

Choose

$$
\mu=\frac3{\sqrt{21}}>0,\qquad \lambda=\frac{3(\sqrt{21}-4)}{5\sqrt{21}}>0,\qquad \nu=1+\lambda>0.
$$

The coefficient of $z$ vanishes, and $2\mu x^*+2\lambda=0$, $2\mu y^*+3-\lambda=0$. Therefore [completing the square](../../../../../../completing-the-square.md) yields

$$
L=3y^*+\mu\bigl((x-x^*)^2+(y-y^*)^2\bigr).
$$

The candidate minimizes $L$ globally and satisfies both active inequality constraints, so [complementary slackness](../../../../../../complementary-slackness.md) and the [Lagrangian sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md) give

$$
\boxed{\min(3y-z)=-\frac{6(1+\sqrt{21})}{5},\quad (x^*,y^*,z^*)=\left(\frac{4-\sqrt{21}}5,-\frac{2+2\sqrt{21}}5,0\right).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
