<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**With excellent [move ordering](../../../../../move-ordering.md), the new horizon is approximately $2d$; without a [move ordering](../../../../../move-ordering.md) assumption, no doubling is guaranteed.** For $b>1$, a full [minimax search](../../../../../minimax-search.md) to depth $d$ visits $\Theta(b^d)$ [search nodes](../../../../../search-node.md), so the budget $n$ has $d\approx\log_b n$. Perfectly ordered [alpha-beta pruning](../../../../../alpha-beta-pruning.md) evaluates only about $\Theta(b^{d'/2})$ leaves at depth $d'$. More precisely, for a complete uniform [game tree](../../../../../game-tree.md), the best leaf count is $b^{\lceil d'/2\rceil}+b^{\lfloor d'/2\rfloor}-1$. Equating the dominant costs gives

$$
b^{d'/2}\approx n\approx b^d,\qquad \boxed{d'\approx2\log_b n\approx2d.}
$$

Constant factors and rounding affect the exact horizon. Poor [move ordering](../../../../../move-ordering.md) can leave the cost at $\Theta(b^{d'})$, giving no asymptotic depth improvement. For $b=1$, there is no branching to prune and the doubling argument does not apply.[§3.2.1, dependence of pruning efficiency on child order](../../../../../cs-188-minimax-notes.md)

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
