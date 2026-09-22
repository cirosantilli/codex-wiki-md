<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Admissible terminal wealth must lie in $(0,\infty)$, the domain of the utility; alternatively extend $U$ by $-\infty$ outside that domain. A one-period [state-price density](../../../../../../state-price-density.md) has $Z>0$ and $\mathbb E[ZP_1]=P_0$, componentwise. Therefore for $W=H\cdot P_1$, $\mathbb E[ZW]=H\cdot P_0=x$.

The dual definition gives the pointwise inequality $U(w)\leq\widehat U(z)+zw$ for $w,z>0$. Apply it with $z=yZ$ and take [expectations](../../../../../../expected-value.md) on the finite state space:

$$
\boxed{\mathbb E U(H\cdot P_1)\leq\mathbb E\widehat U(yZ)+yx.}
$$

Equality holds precisely when $U'(w)=z$, because that is the unique maximizing payoff in the dual definition. If the feasible [portfolio](../../../../../../investment-portfolio.md) $H^*$ has $U'(H^*\cdot P_1)=y^*Z^*$, then

$$
\mathbb E U(H^*\cdot P_1)=\mathbb E\widehat U(y^*Z^*)+y^*x.
$$

The same right side bounds every competing feasible [portfolio](../../../../../../investment-portfolio.md). Thus **$H^*$ is optimal.** This is the [one-period marginal-utility certificate of optimality](../../../../../../one-period-marginal-utility-certificate-of-optimality.md); it does not require the erroneous second-differentiability assertion in part (a).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
