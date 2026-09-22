<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the monotone grand coupling in every coordinate: at each step use the same attempted move for chains started from the bottom and top states, censoring moves that leave the interval. The two copies coalesce after the lower copy has accumulated enough upward drift and boundary censoring has removed their initial separation. Away from the boundary, one step has mean displacement

$$
\frac13-\frac16=\frac16.
$$

Standard exponential concentration for sums of bounded independent increments shows that for every fixed $C>6$ the one-coordinate coupling time $\tau$ satisfies

$$
\mathbb P(\tau>Cn)\leq e^{-c_Cn}.
$$

All other initial states lie between the extremal copies. Coupling the $d$ coordinates independently and using the [union bound](../../../../../../boole-s-inequality.md) gives

$$
\mathbb P(\text{some coordinate has not coupled by }Cn)
\leq d e^{-c_Cn}=o(1),
$$

because $\log d=o(n)$. The [coupling inequality for total variation](../../../../../../coupling-inequality-for-total-variation.md) therefore gives

$$
\boxed{t_{\mathrm{mix}}=O(n).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
