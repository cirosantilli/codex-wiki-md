<h1 id="21h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In this [consecutive-number antisymmetric game](../../../../../../consecutive-number-antisymmetric-game.md), with the row player's number denoted $i$, the [payoff matrix](../../../../../../payoff-matrix.md) is

$$
a_{ij}=\begin{cases}
0,&i=j,\\
1,&i=j+1,\\
-1,&j=i+1,\\
-2,&i\ge j+2,\\
2,&j\ge i+2.
\end{cases}
$$

It is an [antisymmetric matrix](../../../../../../skew-symmetric-matrix.md), so the [matrix game](../../../../../../matrix-game.md) has value zero for every $n\ge3$. For $n=3$,

$$
A=\begin{pmatrix}0&-1&2\\1&0&-1\\-2&1&0\end{pmatrix},\qquad
p=q=\left(\frac14,\frac12,\frac14\right)
$$

satisfies $Ap=0$ and $p^TA=0$, proving optimality for both players.

For any larger $n$, extend the same strategy by zero probabilities:

$$
\boxed{v=0,\qquad p=q=\left(\frac14,\frac12,\frac14,0,\ldots,0\right).}
$$

Indeed, the first three coordinates of $Ap$ are zero. For $i=4$, $(Ap)_4=-2/4-2/2+1/4=-5/4$; for $i\ge5$, all three supported numbers are at least two below $i$, so $(Ap)_i=-2$. Hence $Ap\le0$ and, by antisymmetry, $p^TA\ge0$. The column player using $p$ prevents positive payoff, while the row player using $p$ prevents negative payoff, a [mixed-strategy optimality certificate for a matrix game](../../../../../../mixed-strategy-optimality-certificate-for-a-matrix-game.md). This explicitly checks all the additional strategies rather than assuming the three-number subgame remains optimal.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
