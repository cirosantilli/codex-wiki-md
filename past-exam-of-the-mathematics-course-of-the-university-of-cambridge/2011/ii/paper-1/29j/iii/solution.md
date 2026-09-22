<h1 id="29j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume $S_0\ne0$ and keep $d=S_0^TMS_0>0$, $\eta=(S_0^TM\mu-w_0)/d$. The constraint $x\geq0$ is $S_0^T\theta\leq w_0$. If the unrestricted optimum in (i) lies in this half-space, it remains optimal. Its cash holding is

$$
x_{\rm free}=w_0-S_0^TM\mu+Rd=d(R-\eta).
$$

Thus it has strictly positive cash precisely when $\eta<R$. If $\eta>R$, the free optimum violates the constraint, so strict concavity and the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) put the optimum on the boundary, where it is the cash-free solution in (ii). At equality the two solutions coincide. Therefore

$$
\boxed{\theta^*=M[\mu-\max(R,\eta)S_0],\qquad x^*=\max(0,w_0-S_0^TM\mu+Rd).}
$$

In particular,

$$
\boxed{x^*=0\iff\frac{S_0\cdot(\gamma V)^{-1}\mu-w_0}{S_0\cdot(\gamma V)^{-1}S_0}\geq1+r.}
$$

The multiplier for the inequality is $\max(0,\eta-R)$, explicitly checking the complementary-slackness condition.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [29J](../../29j.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
