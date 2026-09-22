<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Associate nonnegative [Lagrange multipliers](../../../../../../../lagrange-multiplier.md) $\alpha$ with $-Pz-\mathbf1\le0$ and $\beta$ with $Pz-\mathbf1\le0$. The [Lagrangian dual problem](../../../../../../../lagrangian-dual-problem.md) is obtained from

$$
L(z,\alpha,\beta)=r_0^Tx-\mathbf1^T(\alpha+\beta)
+[x-P^T(\alpha-\beta)]^Tz.
$$

Its infimum over unrestricted $z$ is finite exactly when $P^T(\alpha-\beta)=x$. Thus the dual is

$$
\boxed{\sup_{\alpha,\beta\ge0}\ r_0^Tx-\mathbf1^T(\alpha+\beta)
\quad\text{subject to }P^T(\alpha-\beta)=x.}
$$

The precise finiteness condition is $x\in\operatorname{range}P^T$. If $x=P^Tq$, then $x^Tz=q^TPz\ge-\|q\|_1$ on the feasible set. The primal is feasible and bounded below, and splitting $q$ into positive and negative parts makes the dual feasible. [Linear programming duality](../../../../../../../linear-programming-duality.md) therefore gives attained equal finite optima. Equivalently, the strictly feasible point $z=0$ satisfies the [Slater condition](../../../../../../../slater-s-condition.md), with the required finiteness hypothesis. This is [strong duality](../../../../../../../strong-duality.md) in the usual finite sense.

If $x\notin\operatorname{range}P^T=(\ker P)^\perp$, there is $d\in\ker P$ with $x^Td<0$. Every $z=td$, $t\ge0$, is feasible and the objective tends to $-\infty$. The dual is then infeasible. Equality of extended values still holds if its supremum over the empty feasible set is defined as $-\infty$, but there are no finite optimizers. The paper does not assume full column rank of $P$, so this qualification is necessary. The same calculation gives the [support function of an inverse image of an infinity-norm ball](../../../../../../../support-function-of-an-inverse-image-of-an-infinity-norm-ball.md), $\inf_r r^Tx=r_0^Tx-\min_{P^Tq=x}\|q\|_1$ for finite decisions.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
