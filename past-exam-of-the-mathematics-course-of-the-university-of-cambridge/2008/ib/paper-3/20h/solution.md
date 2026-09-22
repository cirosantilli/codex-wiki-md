<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Set $y=x_3+5$, so $y\ge0$ and $y\le10$. Introduce nonnegative slack and surplus variables $s_1,s_2,s_3$:

$$
x_1+x_2+y+s_1=12,\qquad 2x_2+y-s_2=6,\qquad y+s_3=10.
$$

The objective is $z=x_1+2x_2-6y+30$. A feasible [simplex basis](../../../../../simplex-basis.md) is $(x_2,s_1,s_3)$ with nonbasic variables $(x_1,s_2,y)=0$; its basic values are $(3,9,10)$. The initial [simplex dictionary](../../../../../simplex-dictionary.md) is

$$
\begin{aligned}
x_2&=3+\tfrac12s_2-\tfrac12y,\\
s_1&=9-x_1-\tfrac12s_2-\tfrac12y,\\
s_3&=10-y,\\
z&=36+x_1+s_2-7y.
\end{aligned}
$$

In the [simplex algorithm](../../../../../simplex-algorithm.md), choose $s_2$ as the entering variable since it has positive objective coefficient. With the other nonbasic variables zero, only $s_1$ decreases; the [simplex ratio test](../../../../../simplex-ratio-test.md) gives $s_2\le18$. Thus $s_1$ leaves. Pivoting its row gives

$$
\begin{aligned}
s_2&=18-2x_1-y-2s_1,\\
x_2&=12-x_1-y-s_1,\\
s_3&=10-y,\\
z&=54-x_1-8y-2s_1.
\end{aligned}
$$

All nonbasic variables are nonnegative, and all objective coefficients in the final dictionary are nonpositive, proving optimality. Setting them to zero gives $x_1=0$, $y=0$, $x_2=12$, hence

$$
\boxed{(x_1,x_2,x_3)=(0,12,-5),\qquad\max(x_1+2x_2-6x_3)=54.}
$$

The surplus value is $s_2=18$, so the lower constraint is indeed satisfied, not mistakenly treated as equality at the optimum. The strict negative objective coefficients also show uniqueness of the optimizer.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
