<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The players are the two chains, each with the [set](../../../../../set-split.md) of [pure strategies](../../../../../pure-strategy.md) $\{1,2,3,4,5\}$. A [strategy profile](../../../../../strategy-profile.md) $(x,y)$ gives the sites of $S$ and $C$. For later use, write the first player's [payoff](../../../../../payoff.md) for a general street size as

$$
u(x,y)=\begin{cases}x+y-1,&x<y,\\k,&x=y,\\2k-x-y+1,&x>y.\end{cases}
$$

When $x<y$, count customers to the left of $(x+y)/2$, assigning value one rather than two to any midpoint customer. This gives $x+y-1$ whether the midpoint is an occupied building or lies between buildings. The other player receives $2k-u(x,y)$. At co-location, every customer's value is split, giving $k$ each.

For $k=5$, the [payoff matrix](../../../../../payoff-matrix.md) for $S$ is

$$
M=\begin{pmatrix}
5&2&3&4&5\\
8&5&4&5&6\\
7&6&5&6&7\\
6&5&4&5&8\\
5&4&3&2&5
\end{pmatrix}.
$$

Rows and columns are indexed by sites $1,\ldots,5$; the full ordered [payoff](../../../../../payoff.md) pair in cell $(x,y)$ is **$(M_{xy},10-M_{xy})$**. This [discrete location game](../../../../../discrete-location-game.md) is a [constant-sum game](../../../../../constant-sum-game.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
