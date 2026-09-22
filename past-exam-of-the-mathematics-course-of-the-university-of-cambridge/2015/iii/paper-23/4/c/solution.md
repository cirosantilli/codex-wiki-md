<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the one-relation language $\{<\}$ and the [total orders](../../../../../../total-order.md)

$$
\mathcal M=(\mathbb N,<),\qquad \mathcal N=(\mathbb N+\mathbb Z,<),
$$

where the second is the [order sum](../../../../../../order-sum.md): every point in its natural-number block lies below every point in its integer block.

To show II wins every finite [Ehrenfeucht-Fraïssé game](../../../../../../ehrenfeucht-fraisse-game.md), use the [interval threshold strategy for discrete linear orders](../../../../../../interval-threshold-strategy-for-discrete-linear-orders.md). With $k$ rounds left, corresponding open intervals and end rays between already matched points have either the same size below $h_k=2^k-1$, or both have at least $h_k$ elements. Their sizes may be infinite. The chosen-point correspondence is order preserving. Initially the unique interval is infinite in both orders, so the invariant holds.

If I chooses a repeated point, II repeats its counterpart. If I chooses in a short interval, II chooses the point with the same finite rank in the matching interval. In a long interval, let $h=h_{k-1}$. If one side of the chosen point has fewer than $h$ elements, reproduce that size in the other interval; the opposite sides then both have at least $h$ elements. Otherwise choose a response having at least $h$ elements on each side. Such a response exists because the interval has at least $2h+1=h_k$ elements. The endpoint and successor/predecessor properties of these two discrete orders allow the finite small-side counts to be reproduced. This establishes the invariant with $k-1$ rounds left and gives a finite-game winning strategy. Therefore II wins the timed game.

In the infinite [Ehrenfeucht-Fraïssé game](../../../../../../ehrenfeucht-fraisse-game.md), I first chooses a point $b$ in the integer block of $N$. It has infinitely many predecessors. II must respond with some $m\in\mathbb N$, which has exactly $m$ predecessors. I then chooses $m+1$ distinct predecessors of $b$. To preserve order and equality, II would need $m+1$ distinct points below $m$, which is impossible. Thus

$$
\boxed{\text{II wins every announced finite horizon, but I wins }G_\omega.}
$$

I chooses the required finite length only after seeing II's first response, which explains why this does not contradict the timed-game result.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
