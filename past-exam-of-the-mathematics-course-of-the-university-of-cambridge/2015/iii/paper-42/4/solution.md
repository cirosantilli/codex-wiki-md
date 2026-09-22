<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

First exclude boundary profiles. At $(0,0)$, player $i$ can replace its payoff $v_i/2$ by $v_i-\varepsilon^2>v_i/2$ using a sufficiently small positive effort. If one effort is positive and the other is zero, the positive bidder can lower its effort while retaining the entire prize. Thus a pure [Nash equilibrium](../../../../../nash-equilibrium.md) of this [proportional allocation contest](../../../../../proportional-allocation-contest.md) must have both efforts positive.

Against $b_j>0$, player $i$'s payoff is a [strictly concave function](../../../../../strictly-concave-function.md) of $b_i\geq0$, since

$$
\frac{\partial^2 s_i}{\partial b_i^2}
=-\frac{2v_i b_j}{(b_i+b_j)^3}-2<0.
$$

Its derivative at zero is positive and its payoff tends to negative infinity as its own effort tends to infinity. Hence its unique [best response](../../../../../best-response.md) is the positive solution of the [first-order condition](../../../../../first-order-optimality-condition.md). At an equilibrium, writing $B=b_1+b_2$, these conditions are

$$
\frac{v_1b_2}{B^2}=2b_1,\qquad
\frac{v_2b_1}{B^2}=2b_2.
$$

Dividing them gives $b_1/b_2=\sqrt{v_1/v_2}$, and multiplying them gives $B^4=v_1v_2/4$. Therefore the [quadratic-cost two-player proportional contest](../../../../../quadratic-cost-two-player-proportional-contest.md) has

$$
\boxed{B=\frac{(v_1v_2)^{1/4}}{\sqrt2},\qquad
b_i^*=\frac{\sqrt{v_i}}{\sqrt{v_1}+\sqrt{v_2}}\,
\frac{(v_1v_2)^{1/4}}{\sqrt2}.}
$$

Both efforts are positive, and [strict concavity](../../../../../strict-concavity.md) makes them global [best responses](../../../../../best-response.md). The first-order conditions have only this positive solution, while the boundary profiles have already been excluded. This proves both existence and uniqueness. The resulting [winning probabilities](../../../../../winning-probability.md) are $x_i^*=\sqrt{v_i}/(\sqrt{v_1}+\sqrt{v_2})$; for equal values $v$, each effort is $\sqrt{v/8}$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
