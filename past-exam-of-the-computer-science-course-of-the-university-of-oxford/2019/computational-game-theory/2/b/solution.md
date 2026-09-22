<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The row player's unique [best response](../../../../../best-response.md) to $L$ is $B$ and to $R$ is $T$. The column player's unique [best response](../../../../../best-response.md) to $T$ is $R$ and to $B$ is $L$. Thus **the pure [Nash equilibria](../../../../../nash-equilibrium.md) are $(T,R)$ and $(B,L)$**.

For a fully mixed equilibrium, let $p=\Pr(T)$ and $q=\Pr(L)$. Row-player indifference requires

$$
q+3(1-q)=6q+2(1-q),\qquad q=1/6.
$$

Column-player indifference requires

$$
3(1-p)=6p+2(1-p),\qquad p=1/7.
$$

Both [probabilities](../../../../../probability.md) lie strictly between zero and one, so these indifference conditions make both supported actions [best responses](../../../../../best-response.md). Hence the remaining equilibrium is

$$
\boxed{(\Pr(T),\Pr(B))=(1/7,6/7),\qquad(\Pr(L),\Pr(R))=(1/6,5/6).}
$$

Its [expected payoffs](../../../../../expected-payoff.md) are $(8/3,18/7)$. There are no other partly mixed equilibria: if either player is pure, the other's [best response](../../../../../best-response.md) is unique, forcing both to be pure. If both mix, the displayed linear indifference equations uniquely determine their [probabilities](../../../../../probability.md). The row player's equilibrium mixture differs from its maxmin mixture in part (a); these are different optimization criteria in this non-zero-sum game.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
