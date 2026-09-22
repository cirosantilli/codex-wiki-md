<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Reflection in $L$ interchanges $x$ and $y$. Relabel the two points if necessary so that $x$ lies on the side of $L$ containing the center $a$; the absolute difference is symmetric in $x$ and $y$. Couple a Brownian motion $B$ started at $x$ to one $B'$ started at $y$ by setting $B'_t=\phi(B_t)$ before $T_L$ and $B'_t=B_t$ afterwards. The [Brownian reflection coupling](../../../../../../brownian-reflection-coupling.md) has the correct marginal laws because reflection is an isometry and the [Strong Markov property](../../../../../../strong-markov-property.md) applies at $T_L$. Once the paths meet on $L$, they agree forever.

If the path from $x$ does not hit the target circle before $T_L$, the coupled paths meet before the relevant uncoupled hitting outcomes can differ. The [coupling inequality for total variation](../../../../../../coupling-inequality-for-total-variation.md) therefore gives

$$
\boxed{\left|\mathbb P_x(B_{\tau_{a,r_1}}\in A)
-\mathbb P_y(B_{\tau_{a,r_1}}\in A)\right|
\leq\mathbb P_x(\tau_{a,r_1}<T_L).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
