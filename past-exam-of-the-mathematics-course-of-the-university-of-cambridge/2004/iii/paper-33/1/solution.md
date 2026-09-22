<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [linear program](../../../../../linear-programming.md) in maximization form, a nonnegative multiplier $y$ of the resource inequalities gives

$$
c^Tx\leq y^TAx\leq y^Tb
$$

whenever $A^Ty\geq c$. Equivalently, the [Lagrangian](../../../../../lagrangian.md) is $b^Ty+(c-A^Ty)^Tx$; its supremum over $x\geq0$ is finite exactly when $A^Ty\geq c$. Minimizing this bound gives the [dual linear program](../../../../../dual-linear-program.md)

$$
\boxed{\min b^Ty,\qquad A^Ty\geq c,\qquad y\geq0.}
$$

The displayed inequality proves [weak duality](../../../../../weak-duality.md) directly.

For the final [simplex tableau](../../../../../simplex-tableau.md), the basic-variable order is $(x_2,x_1)$. With $z_1,z_2$ interpreted as the ordinary unpriced [slack variables](../../../../../slack-variable.md), its constraint equations give

$$
x_2=1-\frac{z_1+z_2}{10},\qquad
x_1=2-\frac{z_1+3z_2}{20}.
$$

The bottom row is read in the reduced-cost convention $r_j=c_j-c_B^TB^{-1}A_j$, with right side minus the basic objective value. It says the [reduced costs](../../../../../reduced-cost.md) of $z_1,z_2$ are $0,-1/2$. Thus optimality requires $z_2=0$, while $z_1$ can increase without changing the objective until $x_2$ reaches zero. The complete primal optimum set is

$$
\boxed{x_1=2-\frac{\theta}{20},\qquad
x_2=1-\frac{\theta}{10},\qquad0\leq\theta\leq10.}
$$

[Reconstructing a linear program from a final simplex tableau](../../../../../reconstructing-a-linear-program-from-a-final-simplex-tableau.md) exposes a source inconsistency. The slack columns are

$$
B^{-1}=\begin{pmatrix}1/10&1/10\\1/20&3/20\end{pmatrix},
\qquad
B=\begin{pmatrix}15&-10\\-5&10\end{pmatrix}.
$$

Because the first basic column is that of $x_2$, the original constraint data are

$$
A=\begin{pmatrix}-10&15\\10&-5\end{pmatrix},
\qquad b=B\binom12=\binom{-5}{15}.
$$

The slack [reduced costs](../../../../../reduced-cost.md) give $y^T=(0,1/2)$ and

$$
(c_2,c_1)=y^TB=(-5/2,5).
$$

Consequently the recovered homogeneous [linear program](../../../../../linear-programming.md) is

$$
\boxed{\max\left(5x_1-\frac52x_2\right),\qquad
-10x_1+15x_2\leq-5,\quad
10x_1-5x_2\leq15,\quad x_1,x_2\geq0.}
$$

Every point in the optimum segment has value $15/2$. Since the segment contains a point with both variables positive, [complementary slackness](../../../../../complementary-slackness.md) forces both dual column inequalities to be equalities. They give the unique dual optimum

$$
\boxed{y_1=0,\qquad y_2=\frac12,\qquad b^Ty=\frac{15}{2}.}
$$

The printed bottom-right entry is $-3$, but it must be $-15/2$ for this linear objective and these constraint rows. Thus **no original problem in the stated homogeneous standard form has exactly the entire printed tableau**. Changing that one entry to $-15/2$ gives the reconstructed problem above. Alternatively, if an affine objective is permitted, $5x_1-\tfrac52x_2-\tfrac92$ has the displayed optimum value $3$ and unchanged [reduced costs](../../../../../reduced-cost.md); the corresponding affine dual objective is $b^Ty-\tfrac92$. Both interpretations have exactly the same primal and dual optimizer sets. The discrepancy is in the objective constant, not in the optimal segment.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
