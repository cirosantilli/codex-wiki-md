<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If a player chooses site $x$, the opponent can co-locate and hold its [payoff](../../../../../payoff.md) to $k$. Among opposing sites to its right, the lowest [payoff](../../../../../payoff.md) is obtained against $x+1$, giving $2x$. Among opposing sites to its left, the lowest is against $x-1$, giving $2(k-x+1)$. Thus the pure-action [security level payoff](../../../../../security-level-payoff.md) is

$$
g(x)=\min\{k,\,2x,\,2(k-x+1)\}.
$$

The expression remains valid at an endpoint, where the missing-side term is redundant. It reaches its largest possible value $k$ exactly when $k/2\leq x\leq k/2+1$. Hence the pure maxmin [strategies](../../../../../strategy-in-an-infinite-game.md) are

$$
\boxed{\begin{cases}x=(k+1)/2,&k\text{ odd},\\x\in\{k/2,k/2+1\},&k\text{ even},\end{cases}\qquad\text{with guaranteed payoff }k.}
$$

Reflection gives the same answer for the other player.

## ↑ Ancestors (11)

1. [D](../d.md)
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
