<h1 id="5h/solution">Solution</h1>

↑ **Parent:** [5H](../5h.md)

Player A maximizes the [payoff](../../../../../payoff.md), while B minimizes it. The fourth row is strictly worse for A than the first in every column, so remove $A_4$ by [dominated strategy elimination](../../../../../dominated-strategy-elimination.md). On the remaining rows, column $B_3$ is strictly better for B than $B_2$, so remove $B_2$. Now $A_3$ is strictly worse than $A_2$ in the two remaining columns. The reduced [zero-sum game](../../../../../zero-sum-game.md) has [payoff matrix](../../../../../payoff-matrix.md)

$$
\begin{pmatrix}4&-5\\-2&3\end{pmatrix},
$$

with rows $A_1,A_2$ and columns $B_1,B_3$.

If A uses [mixed strategy](../../../../../mixed-strategy.md) $(p,1-p)$, the expected [payoffs](../../../../../payoff.md) against these columns are $-2+6p$ and $3-8p$. The first increases and the second decreases, so their minimum is maximized where they are equal: $14p=5$. Thus

$$
\boxed{A:\ (5/14,9/14,0,0),\qquad v=1/7.}
$$

For an optimality certificate, B uses [mixed strategy](../../../../../mixed-strategy.md) $(q,0,1-q)$, making A's first two row [payoffs](../../../../../payoff.md) $-5+9q$ and $3-5q$. Equality gives $q=4/7$. Against this B strategy the four row [payoffs](../../../../../payoff.md) are $(1/7,1/7,-6/7,-6/7)$, while against the displayed A strategy the three column [payoffs](../../../../../payoff.md) are $(1/7,13/7,1/7)$. Therefore A guarantees $1/7$ and B holds A to $1/7$, verifying the [value of a zero-sum game](../../../../../value-of-a-zero-sum-game.md) and the original, unreduced [mixed strategy](../../../../../mixed-strategy.md).

## ↑ Ancestors (10)

1. [5H](../5h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
