<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With $g=2x-y-z-2$ and $h=x^2+y^2-5$, the maximization [optimization Lagrangian](../../../../../../optimization-lagrangian.md) is

$$
L=-2\lambda x+(3+\lambda)y+(\lambda-1)z-\mu(x^2+y^2-5)+2\lambda.
$$

A finite unconstrained maximum requires $\lambda=1$ to cancel the coefficient of $z$. With $\mu=1$, [completing the square](../../../../../../completing-the-square.md) gives

$$
L=12-(x+1)^2-(y-2)^2.
$$

Thus its global maximizers have $x=-1$ and $y=2$. The equality constraint holds, and [complementary slackness](../../../../../../complementary-slackness.md) with $\lambda=1$ makes $g=0$, giving $z=-6$. The [Lagrangian sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md) certifies

$$
\boxed{(x^*,y^*,z^*)=(-1,2,-6),\qquad \max(3y-z)=12.}
$$

Every feasible point has objective at most $L\leq12$, so this is a global conclusion rather than just a stationary-point calculation.

## ↑ Ancestors (11)

1. [B](../b.md)
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
