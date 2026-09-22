<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $x^*$ maximize SYSTEM. Under the usual positive-capacity, nonempty-route assumptions, the feasible set is compact, contains a positive point, and has a [Slater condition](../../../../../../slater-s-condition.md) point. Strict [concavity](../../../../../../concave-function.md) makes the optimum unique. The condition $U_r'(0)=\infty$ forces $x_r^*>0$: moving from any optimum with a zero component slightly toward a positive feasible point gives an infinite positive directional derivative in that component and only finite losses in the positive components.

By the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md), there are link [Lagrange multipliers](../../../../../../lagrange-multiplier.md) $p_j^*\geq0$ with

$$
U_r'(x_r^*)=(A^Tp^*)_r,\qquad p_j^*\bigl(C_j-(Ax^*)_j\bigr)=0.
$$

Set the [route congestion price](../../../../../../route-congestion-price.md) $y_r^*=(A^Tp^*)_r=U_r'(x_r^*)$ and choose

$$
\boxed{\nu_r^*=x_r^*e^{y_r^*}.}
$$

Then $x_r^*=\nu_r^*e^{-y_r^*}$, as required. For USER with fixed $y_r^*$, the substitution $x=\nu_r e^{-y_r^*}$ is a bijection of the nonnegative half-line, and its objective becomes $U_r(x)-y_r^*x$. This is a [strictly concave function](../../../../../../strictly-concave-function.md) whose derivative vanishes at $x_r^*$, so its unique maximizer is $x_r^*$ and the corresponding USER optimizer is $\nu_r^*$.

For NETWORK at $\nu^*$, its objective derivative at $x^*$ is

$$
\log\frac{\nu_r^*}{x_r^*}=y_r^*=(A^Tp^*)_r.
$$

Thus $x^*,p^*$ obey its [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md), with the same feasibility and [complementary slackness](../../../../../../complementary-slackness.md). The NETWORK objective is a [strictly concave function](../../../../../../strictly-concave-function.md), so $x^*$ is also its unique maximizer. **The triple $(x^*,y^*,\nu^*)$ solves all three problems simultaneously.** This is a [user-network decomposition of concave utility maximization](../../../../../../user-network-decomposition-of-concave-utility-maximization.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
